<!--
name: 'Tool Result: Bash shell-expandable pattern unchecked'
description: >-
  Too-complex reason when a command word has a glob pattern the shell may
  expand, so the command cannot be checked before it runs; becomes the Bash
  permission ask message
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_BASH_SHELL_EXPANDABLE_PATTERN_UNCHECKED_VAR_0
  - TOOL_RESULT_BASH_SHELL_EXPANDABLE_PATTERN_UNCHECKED_VAR_1
  - TOOL_RESULT_BASH_SHELL_EXPANDABLE_PATTERN_UNCHECKED_VAR_2
-->
'${TOOL_RESULT_BASH_SHELL_EXPANDABLE_PATTERN_UNCHECKED_VAR_0} ${TOOL_RESULT_BASH_SHELL_EXPANDABLE_PATTERN_UNCHECKED_VAR_1(TOOL_RESULT_BASH_SHELL_EXPANDABLE_PATTERN_UNCHECKED_VAR_2)}' has a pattern the shell may expand, so this command can't be checked before it runs
