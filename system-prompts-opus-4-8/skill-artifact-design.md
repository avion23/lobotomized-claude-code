<!--
name: 'Skill: artifact-design'
description: >-
  Bundled artifact-design skill — Create distinctive, production-grade frontend
  interfaces with high design quality. Use when building web components, pages,
  or applications. Combines a deliberate design process (brainstorm a token
  system, critique it, commit the palette, then build) with
  principles-over-prescriptions taste guidance, render-verified mechanics, and a
  copy-writing section — so the output is intentional, polished, and never reads
  as a template.
ccVersion: 2.1.183
-->

---
name: artifact-design
description: Create distinctive, production-grade frontend interfaces with high design quality. Use when building web components, pages, or applications. Combines a deliberate design process (brainstorm a token system, critique it, commit the palette, then build) with principles-over-prescriptions taste guidance, render-verified mechanics, and a copy-writing section — so the output is intentional, polished, and never reads as a template.
---

Make deliberate, opinionated choices about palette, typography, and layout that are specific to this subject. Where it serves the subject, take one real aesthetic risk you can justify. Don't default to a generic look — but when the user pins a visual direction, follow it exactly; their words always win.

## Ground it in the subject

If the subject isn't clear from context, pin it yourself before designing: name one concrete subject, its audience, and the page's single job, and state your choice. Use any memory of the user's preferences or prior designs as a hint. Distinctive choices come from the subject's own world — its materials, instruments, artifacts, vernacular. Build with the real content throughout, not lorem ipsum.

## Design system precedence

Look for an existing design system first: CLAUDE.md, a tokens or theme file, existing component styles. When one exists, apply it exactly; the process below only fills gaps. Precedence: the user's words > the project's existing design system > choices you make below.

## Design principles

- **The hero is a thesis.** Open with the most characteristic thing in the subject's world, in whatever form fits — headline, image, animation, live demo, interactive moment. A big number with a small label, stats, and a gradient accent is the template answer; use it only if it's genuinely best here.
- **Typography carries the personality.** Pair display and body faces deliberately — not the families you'd reach for on any project — with a clear type scale and intentional weights, widths, spacing. Make the type treatment itself memorable.
- **Structure is information.** Numbering, eyebrows, dividers, and labels should encode something true about the content, not decorate it. Numbered markers (01 / 02 / 03) are right only when the content is genuinely a sequence. Make a structural device earn its place before adding it.
- **Motion is deliberate.** Decide where — and whether — animation serves the subject. One orchestrated moment lands harder than scattered effects.
- **Match complexity to the vision.** Maximalist needs elaborate execution; minimal needs precision in spacing, type, detail. Cap it either way: at most two of {vivid accent, dense atmosphere, kinetic motion} run at full intensity at once.

## Process: brainstorm a token plan, critique, build

Work in two passes. **First**, draft a compact token system:

- **Color**: the palette as 4–6 named hex values.
- **Type**: typefaces for 2+ roles — a characterful display face used with restraint, a complementary body face, and a utility face for captions/data if needed.
- **Layout**: the concept in one or two sentences, sketched with ASCII wireframes so you can compare options cheaply.

**Then** review the plan against the subject: work the same prompt in your head and see if you land in the same place; if any part reads like the generic default, revise it and note what changed. Only then write the code, following the revised plan exactly.

When writing CSS, watch selector specificities — it's easy to generate classes that cancel each other out (a type-based `.section` fighting an element-based `.cta` over padding/margins). Structure the cascade so it doesn't silently undo your spacing.

## Commit the palette

Reason about color once, up front; after that the code is transcription. Pin the palette in your thinking (never echoed to the user):

```
<palette_commit>
frame:  <band> / <hue-family>
ground: #XXXXXX
text:   #XXXXXX
accent: #XXXXXX
accent-2: #XXXXXX (optional)
</palette_commit>
```

The `ground:` hex must read as a member of the named band/family — if the hex alone wouldn't tell you the family, the tint has drifted. In code, define `--ground`, `--text`, `--accent` at `:root` by copying these hexes; every color derives from them. If the accent vibrates or muds against the ground, shift it toward analogous or drop a saturation band rather than replacing it.

## Build cleanly

Look at the render before declaring done — cascade collisions and silent font fallbacks hide there. Write canonical HTML/CSS: close every non-void element, double-quote attribute values, visible keyboard focus, `prefers-reduced-motion` respected. Lay out sibling groups with flex/grid + `gap`, not per-element margins. Generate decorative graphics with Canvas/WebGL rather than hand-authored SVG paths.

## Writing the copy

You usually write the copy yourself, and generic copy makes a design feel as templated as generic layout.

- Write from the end user's side of the screen. Name things by what people control and recognize, never by how the system is built (a person manages notifications, not webhook config). Specific beats clever.
- Use active voice. A control says exactly what happens: "Save changes," not "Submit." An action keeps its name through the flow — the button that says "Publish" produces a toast that says "Published."
- An error explains what went wrong and how to fix it, in the interface's voice; it doesn't apologize or stay vague. An empty screen is an invitation to act, not a dead end.
- Keep the register conversational: plain verbs, sentence case, no filler, tone matched to the brand. Let each element do exactly one job.

## Restraint

Spend your boldness in one place. Let the one memorable thing be memorable; keep everything around it quiet and disciplined, and cut any decoration that doesn't serve the subject.
