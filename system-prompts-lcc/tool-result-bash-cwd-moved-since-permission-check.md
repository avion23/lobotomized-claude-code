<!--
name: 'Tool Result: Bash cwd moved since permission check'
description: >-
  Error when the working directory no longer leads where it did at the
  permission check, so the command did not run
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_BASH_CWD_MOVED_SINCE_PERMISSION_CHECK_VAR_0
-->
Working directory "${TOOL_RESULT_BASH_CWD_MOVED_SINCE_PERMISSION_CHECK_VAR_0}" no longer leads where it did when this command was permission-checked (a part of the path was replaced, or can't be examined), so this command was not run. Re-issue the command to have it checked afresh.
