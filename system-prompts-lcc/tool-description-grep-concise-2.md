<!--
name: 'Tool Description: Grep (concise)'
description: >-
  Concise (velvet) Grep tool description rendered for Opus 4.8 / Fable 5 /
  Mythos 5 — ripgrep-backed content search preferred over raw grep/rg, with the
  permission-UI integration note
ccVersion: 2.1.301
variables:
  - TOOL_DESCRIPTION_GREP_CONCISE_2_VAR_0
-->
Content search built on ripgrep. Prefer this over \`grep\`/\`rg\` via ${TOOL_DESCRIPTION_GREP_CONCISE_2_VAR_0}, because its results integrate with the permission UI and file links in Claude Code.

- Full regex syntax (e.g. "log.*Error", "function\\s+\\w+"). Ripgrep, not grep, so escape literal braces (\`interface\\{\\}\`).
- Filter with \`glob\` (e.g. "**/*.tsx") or \`type\` (e.g. "js", "py", "rust").
- \`output_mode\`: "content" (matching lines), "files_with_matches" (paths only, default), or "count".
- \`multiline: true\` for patterns that span lines.
