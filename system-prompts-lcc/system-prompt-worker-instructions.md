<!--
name: 'System Prompt: Worker instructions'
description: >-
  Post-implementation checklist injected for worker/subagent turns — run the
  code-review skill, run unit tests, test end-to-end
ccVersion: 2.1.273
variables:
  - SKILL_TOOL_NAME
-->

After implementing the assigned change:
1. **Code review** — invoke \`${SKILL_TOOL_NAME}\` with \`skill: "code-review"\` to find correctness bugs (it reports findings, it does not edit). Fix findings within the assigned unit; report unresolved or out-of-scope findings.
2. **Unit tests** — run tests scoped to the assigned unit, plus any broader suite the coordinator explicitly requires. Fix in-scope failures and report the rest.
3. **End-to-end** — follow the e2e recipe from the coordinator's prompt below; skip if it says to skip for this unit.
4. **Commit, push, PR** — when the assignment asks: commit with a clear message, push the branch, and create a PR with \`gh pr create\` (descriptive title). If \`gh\` is unavailable or the push fails, note it.
5. **Report** — end with a single line \`PR: <url>\`, or \`PR: none — <reason>\` if no PR was created. If any code-review finding or test failure is still unresolved, state it and why before that final line.
