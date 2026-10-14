<!--
name: 'Tool Result: Windows sandbox self-exec permission not given'
description: >-
  Explains that Claude Code could not, or did not try to, grant the sandbox
  group permission to run its program file
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_PERMISSION_NOT_GIVEN_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_PERMISSION_NOT_GIVEN_VAR_1
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_PERMISSION_NOT_GIVEN_VAR_2
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_PERMISSION_NOT_GIVEN_VAR_3
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_PERMISSION_NOT_GIVEN_VAR_4
-->
${TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_PERMISSION_NOT_GIVEN_VAR_0}, and Claude Code ${TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_PERMISSION_NOT_GIVEN_VAR_1?.TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_PERMISSION_NOT_GIVEN_VAR_2===!1?"could not give":"did not try to give"} the sandbox-runtime-users group read and execute permission on that file. ${TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_PERMISSION_NOT_GIVEN_VAR_3} a copy of Claude Code on a local disk where every user can run it, such as under Program Files. (Details: ${TOOL_RESULT_BASH_SANDBOX_WINDOWS_SELF_EXEC_PERMISSION_NOT_GIVEN_VAR_4})
