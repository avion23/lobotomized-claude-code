<!--
name: 'Tool Result: Windows sandbox self-exec blocked despite permission'
description: >-
  Explains that Windows still refused the sandbox account after permission was
  granted and suggests asking an administrator
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_BLOCKED_DESPITE_PERMISSION_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_BLOCKED_DESPITE_PERMISSION_VAR_1
-->
${TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_BLOCKED_DESPITE_PERMISSION_VAR_0}, even though Claude Code gave the sandbox-runtime-users group read and execute permission on that file. Security software or a Windows policy may be blocking it; ask your administrator. (Details: ${TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_BLOCKED_DESPITE_PERMISSION_VAR_1})
