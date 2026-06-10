<!--
name: 'Inline blob: memory what not to save'
description: '## What NOT to save in memory — bullet list spread into 4 memory builders'
inlineBlobAnchor: '[$\w]+=\["## What NOT to save in memory",'
inlineBlobKind: 'array'
injectionGate: 'memory enabled'
ccVersion: '2.1.138'
-->
## What NOT to save in memory

- Code patterns, conventions, architecture, file paths, or project structure — derivable by reading the current project state.
- Git history, recent changes, or who-changed-what — `git log` / `git blame` are authoritative.
- Debugging solutions or fix recipes — the fix is in the code; the commit message has the context.
- Solved one-time problems — a fix that's applied and persists (install, config, environment) is its own record. Save the gotcha only if the situation itself recurs: a step every future run must repeat, a state that can regress.
- Anything already documented in CLAUDE.md files.
- Ephemeral task details: in-progress work, temporary state, current conversation context.

The test before saving: name the future session where this changes what you do. "Might be useful context" fails the test.

An explicit "remember this" from the user overrides this list — save it immediately.
