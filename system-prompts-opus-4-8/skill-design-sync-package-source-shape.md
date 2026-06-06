<!--
name: 'Skill: /design-sync package source shape'
description: >-
  design-sync skill reference shown when no Storybook is present: the component
  list comes from the package’s shipped .d.ts exports and previews are generated
  from .d.ts prop types
ccVersion: 2.1.167
-->
# Package source shape

No Storybook — the component list comes from the package's shipped `.d.ts` exports; previews are generated from the `.d.ts` prop types plus `cfg.previewArgs`.

## 2. Explore, then write config (continued)

3. **Get `dist/` built.** The converter needs the built entry (`package.json` `module`/`main`/`exports['.']`) + its `.d.ts` tree. Install may have built it via `prepare`. If missing:
   - Run `<pm> run build`; no `build` script → `prepare`/`prepack`. In a monorepo, build the package *and its workspace dependencies* from the root: `turbo build --filter=<pkg>` or `pnpm -F "<pkg>..." build` (the trailing `...` is required — bare `-F <pkg>` skips deps → `Cannot find module '@scope/tokens'`). Some build scripts fork a watcher and exit 0 early — after the command returns, `ls` the expected output (`dist/`, `build/esm/`, or whatever `package.json` `module`/`main` points at) and confirm it's populated. If empty, use the script's one-shot (non-`--watch`) variant or poll the output dir.
   - Still missing → `AskUserQuestion`("What command builds this package?", options = `scripts.*` containing `tsc|tsup|rollup|vite build|esbuild|swc`, plus freeform). Record as `buildCmd`.
   - No build at all → the converter synthesizes an entry from `src/` (weaker `.d.ts` contracts; recommend adding a build).
4. **Check the existing project.** `DesignSync(list_files)`. If non-empty, read `_ds_bundle.js` via `DesignSync(get_file)` and note component names from its first-line `/* @ds-bundle: {…} */` header. Still rebuild (step 7) — the existing bundle is stale once source changes; the header's `sourceHashes` diff only decides what to *upload* incrementally.
5. **Confirm the plan before building.** `AskUserQuestion` with: the component list (or count + a few names), the tokens/CSS source files, and the build command. The build can take minutes and burn tokens; aligning now avoids re-running on the wrong package. If the project already has N components, offer scope: (a) full rebuild + re-upload, (b) update only changed components (`sourceHashes` diff), (c) tokens + CSS only. Default to (b) on a small diff.
6. **Write and commit `design-sync.config.json`** — re-sync reuses it for reproducible output. Only `pkg` and `globalName` are required. If the file exists, read it first and preserve `previewArgs`, `dtsPropsFor`, `libOverrides`, `overrides`, and `notes` — only add to those, never replace; they accumulate verify-loop fixes. Read `.design-sync/NOTES.md` (or whatever `cfg.notes` points at) first too — repo-specific gotchas a prior sync recorded.

   | Field | Value |
   |---|---|
   | `pkg` / `globalName` | package name and the `window.*` global — required |
   | `shape` | `'storybook'` or `'package'` — pins the source shape (overrides auto-detection). Written on first run. |
   | `buildCmd` | discovered build command; re-sync re-runs it |
   | `srcDir` | source root when not `src/`/`lib/`/`components/` |
   | `tsconfig` | `tsconfig.json` path — esbuild reads `compilerOptions.paths` so `@/…` aliases resolve in synth-entry mode |
   | `extraEntries` | package names to merge into `window.<globalName>` alongside the DS entry (e.g. a separate icon package). Same-scope sibling icon packages auto-detect (`[ICON_PKG]`). |
   | `componentSrcMap` | sparse `{Name: path}` — non-null pins/adds a component's src path; `null` excludes a `.d.ts`-exported internal |
   | `dtsPropsFor` | `{Name: "prop?: Type; …"}` — hand-written `<Name>Props` body when auto-extraction fails (complex generics, cross-package types) |
   | `previewArgs` | `{Name: {prop: value}}` — props rendered as a `Preview` export in `.design-sync/previews/<Name>.tsx`. Simple flat props only; for composed JSX children edit the `.tsx`. |
   | `cssEntry` / `tokensPkg` / `tokensGlob` | stylesheet + token files |
   | `docsDir` | package-relative dir (may point outside, e.g. `../../apps/docs`) of per-component `.md`/`.mdx` docs. Auto-detects `docs/` or `documentation/`. |
   | `docsMap` | sparse `{Name: path \| null}` — explicit doc path (overrides discovery); `null` excludes |
   | `guidelinesGlob` | string or string[] (package-relative) of design-guideline `.md` files copied into `guidelines/`. Default `['docs/guides/**/*.md', 'docs/*.md', 'guides/**/*.md']`. |
   | `extraFonts` | paths (package-relative; may point outside) to `@font-face` `.css` or bare `.woff2`/`.ttf`/`.otf` for brand families the DS expects the host app to provide. CSS entries are parsed and their local fonts copied to `fonts/`; bare fonts copied as-is. Use on `[FONT_MISSING]`. |
   | `runtimeFontPrefixes` | string[] — family-name prefixes for fonts the host app serves at runtime (no `@font-face` to ship). Suppresses `[FONT_MISSING]` for matching families. |
   | `replaces` | `{<raw-element>: [<ComponentName>]}` — extends the adherence-config raw-element map |
   | `libOverrides` | `{"<name>.mjs": "<reason>"}` — declares which `.design-sync/lib/*.mjs` files this repo forks and why (§Troubleshooting). Cross-checked at build time. |
   | `notes` | path to a markdown notes file — default `"./.design-sync/NOTES.md"`. Repo quirks (workspace build order, flaky stories, odd entry paths), one bullet each. Read first on re-sync; append when you learn something. |

7. **Run the converter.** For large DSes (200+ components) the ts-morph `.d.ts` parse takes minutes; `[DTS]` stderr lines show progress. Stage scripts into `.ds-sync/` and install converter deps there (isolated from the repo's lockfile/package manager):

```bash
mkdir -p .ds-sync && cp -r "<skill-base-dir>"/package-build.mjs "<skill-base-dir>"/package-validate.mjs "<skill-base-dir>"/lib .ds-sync/
echo '{"name":"ds-sync-deps","private":true}' > .ds-sync/package.json
(cd .ds-sync && npm i esbuild ts-morph @types/react)
node .ds-sync/package-build.mjs --config design-sync.config.json --node-modules <pkg-node-modules> \
  --entry ./dist/index.es.js --out ./ds-bundle
node .ds-sync/package-validate.mjs ./ds-bundle
```

Run build and validate as separate commands and check each exit code — a chained `build && validate` backgrounded exits non-zero with no visible log when build fails. In a headless / `-p` session run both synchronously (no `run_in_background`): there's no task-notification re-invocation, so a backgrounded run never resumes. Interactive sessions may background.

In a monorepo, point `--node-modules` at the DS package's own `node_modules` (where its `react` resolves) — not the repo root. `--entry` is needed because `node_modules/<pkg>` usually doesn't self-install in the DS's own repo.

Notes:
- `@types/react` is required for prop extraction — without it `React.ComponentPropsWithoutRef<…>` and similar resolve to `any` and the emitted `.d.ts` loses inherited props (`[DTS_REACT]`).
- Complex monorepo build → `npm install <your-pkg>@latest react react-dom` into a scratch dir and pass `--node-modules <scratch>/node_modules` (published dist, flattened deps).

## What the converter emits

Per component, `components/<group>/<Name>/`: `<Name>.jsx` (re-export stub), `<Name>.d.ts` (props from shipped types), `<Name>.prompt.md`, `<Name>.html` (preview card). The converter writes all of these.

`<Name>.prompt.md` is the matched per-component doc when one exists (sibling `<Name>.md`/`.mdx` → `cfg.docsDir` lookup → `<Name>.stories.mdx`; frontmatter `category` sets `<group>`); otherwise synthesized from the `.d.ts` props, leading JSDoc, and `.design-sync/previews/<Name>.tsx` examples. `[DOCS_UNMAPPED]` lists components that didn't match.

`<Name>.html` renders from `window.<GLOBAL>.<Name>` via the compiled `.design-sync/previews/<Name>.tsx` (each named export = one labeled cell); a failed build falls back to story-grid / `.d.ts`-scaffold paths. Compound components needing composed children: edit `.design-sync/previews/<Name>.tsx` (real JSX, with DS imports) and delete its first-line marker. Hand-edits to `.html` are overwritten on rebuild.

`.design-sync/previews/<Name>.tsx` is auto-generated each run (CSF3 render-fn JSX → story args → `cfg.previewArgs` → `.d.ts` variant grid → namespace stub → default). Line 1 is `// @ds-preview generated <sha12> — …`, the sha12 hashing the body. While the marker is present and the hash matches, the file regenerates; delete the marker to own it (logs `(preview override: <Name>)`). Edit the body but leave the marker → warns `(preview edited under marker: <Name>)` and skips. Commit alongside `design-sync.config.json`, `.design-sync/NOTES.md`, and `.design-sync/lib/`.

## 3. Self-heal loop

`package-validate.mjs` emits `[TAG]`-prefixed diagnostics on stderr. Per error: match the tag → apply the fix → rebuild → re-validate until exit 0. Stories that genuinely can't render statically (interaction-driven, data-fetching) go in `cfg.overrides.<Component>.skip` (inline, or `cfg.overrides` can be a path to a JSON file).

| Tag | Symptom | Fix |
|---|---|---|
| `[NO_DIST]` | `entry <path> doesn't exist` | DS isn't built. Run its build (`npm run build` / `turbo run build`), or the published-dist alternative above. |
| `[WORKSPACE_SIBLING]` | `Could not resolve "<sibling>"` | A workspace sibling isn't built. `turbo build` it, or `npm install` published versions into a scratch dir. |
| `[PNPM_SELF_PROVISION]` | `packageManager: pnpm@X` tries to auto-install and fails | Corepack → `COREPACK_ENABLE_STRICT=0`; npm's own provisioning → `npm_config_manage_package_manager_versions=false`. Retry. |
| `[CONFIG]` | `<path>: <json error>` | `design-sync.config.json` is missing or malformed. Fix the JSON. |
| `[ZERO_MATCH]` | no components discovered | No PascalCase `.d.ts` exports and empty `componentSrcMap`. |
| `[OUT_UNSAFE]` | `refusing to rm <path>` | `--out` points at `/`, `$HOME`, cwd, or a non-empty non-bundle dir. Point it at an empty dir. |
| `[UNRESOLVED_IMPORT]` | `<pkg> missing from node_modules` | A DS dependency isn't installed. Run the repo's install (2.1) or add it. |
| `[DSCARD_MISSING]` | `first line isn't a @dsCard comment` | Preview line 1 must be `<!-- @dsCard group="…" -->` for the DS pane to register it. Usually a local `lib/emit.mjs` edit dropped it — restore or re-run. |
| `[LINK_HREF_MISSING]` | `<link href="…"> doesn't resolve` | Preview stylesheet path doesn't resolve relative to the file. Emit-depth mismatch — re-run; if hand-edited, fix the `../` depth. |
| `[CSS_IMPORT_MISSING]` | `styles.css @imports "…" which doesn't exist` | A scraped CSS file isn't on disk. Check `cfg.cssEntry`/`cfg.tokensGlob` point at real files, re-run. |
| `[PROMPT_EMPTY]` | `first line is empty` | `.prompt.md` line 1 is the element-index summary the design agent reads. Re-run; if still empty, add JSDoc to the source. |
| `[RENDER]` | `root empty` | `<Name>.html` didn't render in headless chromium. Check `.render-check.json` `firstErr`; usually a provider/context not in `cfg.provider`. Data-fetching/interaction-only → `cfg.overrides.<Component>.skip`. |
| `[RENDER_ERRORS]` | `<first pageerror>` | Informational — rendered (root non-empty) but threw `pageerror`(s). Usually a missing provider/context (§Troubleshooting). Non-blocking unless `[RENDER]` also fires. |
| `[RENDER_BLANK]` | `renders but PNG <5KB` | Renders but the auto-JSX produced nothing visible. Add `cfg.previewArgs.<Name>` (see `<Name>.d.ts`); compound components needing composed children → edit `.design-sync/previews/<Name>.tsx` and delete its marker. |
| `[RENDER_THIN]` | `text is just "<Name>"` / `variants identical` | Placeholder-only or every variant the same. Same fix as `[RENDER_BLANK]`. |
| `[CSS_PLACEHOLDER]` | `_ds_bundle.css` is an `@import`-only stub | Set `cfg.cssEntry` to the compiled stylesheet (largest `.css` under `dist/`, or per the package's docs). |
| `[TOKENS_MISSING]` | `N CSS custom properties referenced but not defined` | Non-blocking. Component CSS uses `var(--token-*)` but no shipped stylesheet defines them — usually tokens are in a sibling package. Set `cfg.tokensPkg` to it (build log `[TOKENS_PKG]` auto-detects same-scope `*tokens*`/`*theme*` deps). If injected at runtime by a theme provider, set `cfg.provider` instead. |
| `[CSS_RUNTIME]` | no static CSS; wrote a self-styling `styles.css` | Informational, non-blocking. Expected for CSS-in-JS DSes (self-styling bundle); confirm the render check passes. Set `cfg.cssEntry` only if the DS ships a stylesheet the scrape missed; author other globals (e.g. a remote webfont) into a CSS file and point `cfg.cssEntry` at it. |
| `[FONT_MISSING]` | families referenced with no shipped `@font-face` | Non-blocking. The DS expects the host app to provide brand families. Set `cfg.extraFonts` to the `@font-face` css / woff2s (often a sibling typography package), or accept system-font substitutes. |
| `[DOCS_UNMAPPED]` | `<Name>` — no per-component doc | Informational. Set `cfg.docsDir` or `cfg.docsMap.<Name>`. Unmatched get a synthesized `.prompt.md`. |
| `[FONT_DANGLING]` | `@font-face` shipped but its `url()` target isn't | Non-blocking. The font wasn't copied to `fonts/` — usually an `extraFonts:`/`cssEntry:` skip in the build log. Fix the `cfg.extraFonts` path or copy the woff2 under the DS package. |
| — | Icons render as empty boxes / missing | Icon package isn't bundled. Check the log for `[ICON_PKG]` (same-scope auto-included); if absent, add the icon package to `cfg.extraEntries`. |
| — | Components render, no CSS | Set `cfg.cssEntry` to the package's stylesheet. |
| — | "Missing brand fonts" banner in the DS pane | Same as `[FONT_MISSING]`: wire via `cfg.extraFonts` or accept substitutes. |
| — | `! extraFonts: <path> resolves outside the workspace root — skipped` | `extraFonts` is bounded to `dirname(--node-modules)`. In pnpm-workspace / yarn-nohoist repos where `--node-modules` is the per-package one, a sibling typography package falls outside. Copy the `@font-face` css + woff2s under the DS package and point `extraFonts` there, or re-run with the repo-root `node_modules`. |

## 4. Verify previews render

The headless render check (opens every `<Name>.html`, fails on empty root) needs playwright + chromium. Check for an existing install first — `ls ~/.cache/ms-playwright/` or `which chromium chromium-headless-shell google-chrome`. If a chromium build is cached, install the matching playwright version (dir name is `chromium-<build>`; check the repo's `package.json`/lockfile for a pinned `playwright`/`@playwright/test` and `npm i -D playwright@<that-version>` — `npm view playwright@latest` rarely matches). A mismatch gives `browserType.launch: Executable doesn't exist`.

If not found, `AskUserQuestion` before installing:
> "For automated preview verification I'd install playwright + chromium (~200MB). Options: (a) OK to install, (b) Skip — I'll open previews in my own browser, (c) Skip verification entirely."

- (a) → `npm i -D playwright && npx playwright install chromium`. If install fails (CDN blocked, version mismatch), fall through to (b).
- (b) → `npx serve ds-bundle`, list 5–8 preview paths (mix of simple, compound, overlay) for the user. Ask which looked blank or wrong; add a `cfg.previewArgs.<Name>` per their description and re-run.
- (c) → ship with smart-scaffold defaults; note in the final output that previews weren't visually verified.

When backgrounding a long command (playwright install, the build, a server), capture its PID with `PID=$!` and poll with `kill -0 "$PID"`. Don't `pgrep -f '<command string>'` — pgrep matches its own argument, so the loop never exits.

With playwright available, `package-validate.mjs` screenshots every preview to `ds-bundle/_screenshots/<group>__<Name>.png` and writes per-component status to `ds-bundle/.render-check.json` (`[{name, group, errs, firstErr, pngBytes, blank, rootEmpty, thin, nameOnly, allHollow, collapsed, hasPlaceholder, maxHeight, variantsIdentical, bad, texts}]`). Read it and:

1. **Sweep.** Read `_screenshots/contact-sheets.json`. Missing → the sheet step didn't complete, go to step 2. Otherwise Read every `_screenshots/contact-sheet-N.png` it lists (~16 labeled previews each); note tiles that look off — name-only, empty variant labels, broken, placeholder.
2. **Drill.** For every component that is (a) flagged in `.render-check.json` (`bad`, `thin`, `hasPlaceholder`, or `variantsIdentical` true), (b) looked off in the sweep, or (c) any component if step 1 found no json: Read its individual `_screenshots/<group>__<Name>.png` — judge from the full PNG, not a sheet thumbnail. If it looks right (a Divider is a line, an Icon is a glyph), move on — `thin` is a hint, not a verdict. Otherwise Read `<Name>.d.ts` and either add `cfg.previewArgs.<Name>` (simple flat props) or, for compound components needing composed children or inline fixture data, edit `.design-sync/previews/<Name>.tsx` and delete its `// @ds-preview generated` marker. `hasPlaceholder: true` → the dashed-box placeholder is showing; edit the `.tsx`. `blank: true` (PNG <5KB) → the auto-JSX synthesized nothing. `errs > 0` with a context/provider message → §Troubleshooting. Build log `(preview: <Name> — N renderSource(s) reference undeclared …)` → the story's JSX closes over story-file-local fixtures; inline that data into the `.tsx`.
   `previewArgs` is for flat JSON-serializable props (one extra `Preview` export). Composed children (`<Tabs><Tab/><Tab/></Tabs>`), fixture data, or real JSX → edit the `.tsx` directly; `previewArgs` can't express those. A `firstErr` TypeScript error (`Property '…' is missing`, `Type '…' is not assignable`) → fix the `.tsx`; the generated JSX has the wrong prop shape.
3. Re-run `package-build.mjs` then `package-validate.mjs`. Only the components whose `.tsx` you edited (marker deleted → kept) or whose `previewArgs` you added change; marker-bearing files regenerate.
4. Repeat until the `bad` set is empty or 3 iterations.
5. After the final pass, `DesignSync({method: 'report_validate', counts: {total, bad, thin, variantsIdentical, iterations}})` with the aggregate from `.render-check.json` (`total` = entries; `bad`/`thin`/`variantsIdentical` = count of true; `iterations` = rebuild passes).
6. On `[FONT_MISSING]`: interactive → `AskUserQuestion` whether to wire `cfg.extraFonts` (and rebuild) or accept substitutes; headless → note it and proceed.

Steps 1–5 gate §5 — don't `finalize_plan`/upload until they're complete.

Final output to the user: "N/M previews render cleanly; X fixed via previewArgs; Y still need attention: [names]; reviewed Y/Y flagged previews + S contact sheets." For Y, Read and attach the PNGs.

Also confirm:
- `components:` count matches what the user approved in §2. Shortfall → §Troubleshooting (`componentSrcMap`).
- In the browser console on any preview (`npx serve ds-bundle`), `Object.keys(window.<globalName>)` lists every exported component.

## 5. Upload

Only upload after the converter finishes and `package-validate.mjs` exits 0 — a mid-run snapshot has dangling references. Upload at the DS project root; the self-check expects `_ds_bundle.js`, `styles.css`, `components/`, `tokens/`, `fonts/`, `README.md` at top level.

`touch ds-bundle/_ds_needs_recompile` (empty sentinel).

`DesignSync(finalize_plan)` with `localDir: "./ds-bundle"`, `writes: ["components/**", "tokens/**", "fonts/**", "_vendor/**", "_preview/**", "guidelines/**", "_ds_bundle.js", "_ds_bundle.css", "styles.css", "README.md", "_ds_needs_recompile"]`, and `deletes: []` (required even when empty). Dot-prefixed root entries (`.ds-build-meta.json`, `.ds-bundle`, `.pkg-entry.mjs`, `.bundle-entry.mjs`, `.sb-static/`) and `_screenshots/` stay local; `_vendor/` uploads (preview cards load React from it). Add `"demo.html"` only when `cfg.demo` is set.

`finalize_plan` shows the user an interactive approval prompt. If denied, stop — don't retry with different `localDir`/`writes`; denial means the session can't approve, not that the arguments were wrong. Report the validated `ds-bundle/` path and let the user upload interactively.

As the **first** write after approval, `DesignSync(write_files, [{path: "_ds_needs_recompile", localPath: "_ds_needs_recompile"}])` — this fences the app's manifest/copy machinery during upload so consumers never see a half-uploaded state. Then `DesignSync(write_files)` for every other file in the plan, preserving root-relative paths verbatim. The tool caps at 256 files per call — list the tree, chunk into ≤256-file batches, issue multiple `write_files` calls under one `planId`. After all other uploads complete, write the sentinel again to re-arm the recompile in case the project was opened mid-sync. `DesignSync(list_files)` to confirm the count. Each `<Name>.html` carries a first-line `<!-- @dsCard group="…" -->` comment the app's self-check reads to register cards.

When done, tell the user: the project URL (`https://claude.ai/design/p/<projectId>`), component count, files uploaded, and that validate exited clean. Commit `design-sync.config.json`, `.design-sync/NOTES.md`, and any `.design-sync/lib/` overrides so future runs reuse the `previewArgs`/`dtsPropsFor`/`libOverrides` and notes from the verify loop.

## 6. Self-check (server-side)

Done after upload. The app's self-check fires on project open (the `_ds_needs_recompile` sentinel triggers it), so the DS pane populates within a few seconds. It reads each `<Name>.d.ts` as the API contract, the `@dsCard` line from each `<Name>.html` to register cards, regenerates the adherence config and `ds_manifest` from the uploaded source, and clears the sentinel.

## How it works

**Importable bundle** (root `_ds_bundle.js`): esbuild takes the package's published `dist/` entry → one IIFE assigning every export to `window.<globalName>`, with a first-line `/* @ds-bundle: {…} */` header the self-check reads. Its `_ds_bundle.css` sidecar plus scraped tokens/fonts wire through a root `styles.css` that `@import`s them. Storybook-independent; works on every DS.

The converter does NOT emit the adherence config, `ds_manifest`, a version file, or a barrel `index.js` — the self-check regenerates those.

**Scope:** React design systems. Both `_ds_bundle.js` and the previews render via React; a non-React DS has nothing for the claude.ai/design agent to build with. The customer's shipped code is the source of truth — the agent does discovery, config, and the self-heal tail, never component authoring. Inspect locally with `npx serve ds-bundle`.

## Troubleshooting

**"context"/"provider" errors** ("No <X> context", "use<Hook> must be inside <Provider>") → the DS needs a provider wrapper. Set `cfg.provider` to the DS's top-level provider; for a chain, nest via `inner`:
```json
{"provider": {"component": "ThemeProvider", "props": {"theme": {}}, "inner": {"component": "RouterProvider"}}}
```
Look for exports named `*Provider` or `Theme`, or the DS's docs for "wrap your app in". `component` may be a dotted path into an export (e.g. `"<ExportedContext>.Provider"`).

**Missing/wrong components?** `grep ASSUMPTION lib/*.mjs` — each line names the `cfg.*` field overriding that heuristic. `componentSrcMap` covers most: `{"Portal": null}` excludes an exported internal; `{"TextInput": "src/forms/text-input/index.tsx"}` pins a src path the fuzzy-find missed. Synth-entry mode (no dist, no `.d.ts`) may over-include PascalCase non-components (e.g. `ButtonVariants`) — prune with `componentSrcMap: {"ButtonVariants": null}`.

**Render check on large DSes:** validate screenshots every preview by default. For 200+ components where that's too slow, pass `--render-sample N` (deterministic stride).

**Forking a lib script:** when no config override fits, copy the adapter to `.design-sync/lib/<name>.mjs` and edit it there. `package-build.mjs` checks `.design-sync/lib/` first and logs `[OVERRIDE]`. Add a header `// forked from design-sync lib/<name>.mjs — <reason>`, the same reason to `cfg.libOverrides`, and commit both with the config. A fork's `import './common.mjs'` resolves under `.design-sync/lib/`, so also copy (unchanged) any sibling lib files it imports. On re-sync, diff against the bundled `lib/<name>.mjs` and offer to merge upstream changes. Don't fork `lib/emit.mjs` or `lib/bundle.mjs` — they define the output contract with the self-check; use config overrides or `cfg.dtsPropsFor`.

**Known limitations:**
- `.d.ts` props resolve via the TypeScript checker (ts-morph) — generics, `extends` chains, intersections, type aliases resolve to their structural shape; React and CSS-in-JS style-system props are filtered; upstream type bugs propagate as-is.
- A provider read from context (theme, router, i18n) must be in `cfg.provider`, else the preview renders blank.
- Monorepo with a central `apps/storybook`: set `cfg.storybookConfigDir` to run the storybook shape instead.
- Tokens-only DS (no components): emits `styles.css` only with an empty-bodied `_ds_bundle.js`.

## What this is not

Not an LLM rewriting components. The customer's real shipped code is the source of truth; the converter bundles it deterministically. You (the agent) do discovery, config, and the self-heal tail — never component authoring.
