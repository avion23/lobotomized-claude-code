<!--
name: 'Tool Result: Hook blocking, Git Bash not found'
description: >-
  Explains that a required hook blocks because Git Bash was not found and that
  the user must fix the hook config
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_HOOK_BLOCKING_GIT_BASH_NOT_FOUND_VAR_0
-->
blocking because Git Bash wasn't found and this hook doesn't set "shell" to "powershell", so only exit code 0 or 2 counts as its verdict. ${TOOL_RESULT_HOOK_BLOCKING_GIT_BASH_NOT_FOUND_VAR_0} and start a new session, or set "shell" to "powershell" if the hook is written for PowerShell. The user needs to do this; Claude should not change the hook.
