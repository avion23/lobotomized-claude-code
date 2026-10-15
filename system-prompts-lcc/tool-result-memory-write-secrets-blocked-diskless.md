<!--
name: 'Tool Result: memory write secrets blocked (diskless)'
description: >-
  Write refused because content contains potential secrets and every file of a
  memoryless session is checked as memory
ccVersion: 2.1.301
variables:
  - TOOL_RESULT_MEMORY_WRITE_SECRETS_BLOCKED_DISKLESS_VAR_0
-->
Content contains potential secrets (${TOOL_RESULT_MEMORY_WRITE_SECRETS_BLOCKED_DISKLESS_VAR_0}) and cannot be written. This session has no memory folder, so every file it writes is checked as a memory file would be. Remove the sensitive content and try again.
