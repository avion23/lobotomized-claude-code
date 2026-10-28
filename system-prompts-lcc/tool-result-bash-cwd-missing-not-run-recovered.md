<!--
name: Bash cwd missing recovered
description: >-
  Error that the working directory no longer exists, the command was not run and
  cwd was recovered
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_CWD_MISSING_NOT_RUN_RECOVERED_VAR_0
  - TOOL_RESULT_BASH_CWD_MISSING_NOT_RUN_RECOVERED_VAR_1
-->
Working directory "${TOOL_RESULT_BASH_CWD_MISSING_NOT_RUN_RECOVERED_VAR_0}" no longer exists, so this command was not run. Shell cwd recovered to "${TOOL_RESULT_BASH_CWD_MISSING_NOT_RUN_RECOVERED_VAR_1}": re-issue the command if it still makes sense there.
