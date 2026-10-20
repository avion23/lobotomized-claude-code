<!--
name: 'Tool Result: Bash Linux sandbox too many bwrap arguments'
description: >-
  Error when the Linux sandbox profile has more bwrap arguments than bwrap
  accepts, with an approximate mount count and a breakdown of what the arguments
  come from
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_0
  - TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_1
  - TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_2
-->
Sandbox profile has ${TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_0.length} bwrap arguments and bwrap accepts at most ${TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_1} (about ${TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_1/3} mounts). ${TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_2()}
