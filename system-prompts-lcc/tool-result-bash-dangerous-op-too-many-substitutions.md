<!--
name: 'Tool Result: Bash dangerous operation — too many command substitutions'
description: >-
  Dangerous-removal ask message when a command holding rm has more than 64
  command substitutions, too many to analyze; it needs explicit approval.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_DANGEROUS_OP_TOO_MANY_SUBSTITUTIONS_VAR_0
-->
This command contains ${TOOL_RESULT_BASH_DANGEROUS_OP_TOO_MANY_SUBSTITUTIONS_VAR_0.length} command substitutions — too many to analyze for catastrophic removals. This requires explicit approval.
