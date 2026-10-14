<!--
name: 'Tool Result: Windows sandbox icacls grant remedy'
description: >-
  Tells the owner or an administrator to grant the sandbox group read and
  execute with icacls
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_ICACLS_GRANT_REMEDY_VAR_0
-->
Its owner or an administrator can: in PowerShell or Command Prompt (not Git Bash, which rewrites /grant), run icacls "${TOOL_RESULT_BASH_SANDBOX_WINDOWS_ICACLS_GRANT_REMEDY_VAR_0.execPath}" /grant sandbox-runtime-users:RX (then restart Claude Code). Otherwise use
