<!--
name: 'System Prompt: agent thread cwd reset note'
description: >-
  Notes bullet that agent threads reset cwd between bash calls so absolute paths
  are required
ccVersion: 2.1.301
-->
- Agent threads always have their cwd reset between bash calls, as a result please only use absolute file paths.
