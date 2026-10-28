<!--
name: 'Tool Result: Bash readonly name declared twice'
description: >-
  Ask reason when readonly names the same variable twice so the second
  assignment does not happen
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_BASH_READONLY_NAME_DECLARED_TWICE_VAR_0
  - TOOL_RESULT_BASH_READONLY_NAME_DECLARED_TWICE_VAR_1
  - TOOL_RESULT_BASH_READONLY_NAME_DECLARED_TWICE_VAR_2
-->
${TOOL_RESULT_BASH_READONLY_NAME_DECLARED_TWICE_VAR_0} names '${TOOL_RESULT_BASH_READONLY_NAME_DECLARED_TWICE_VAR_1(TOOL_RESULT_BASH_READONLY_NAME_DECLARED_TWICE_VAR_2)}' twice — the first makes it read-only, so bash does not carry out the second
