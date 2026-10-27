<!--
name: 'Bash: one-command assignment behind a failable expansion'
description: >-
  Permission reason when a prefix assignment rides a command whose expansion can
  fail at runtime
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_DECLARATION_EXPANSION_UNVERIFIABLE_PREFIX_ASSIGN_VAR_0
-->
'${TOOL_RESULT_BASH_DECLARATION_EXPANSION_UNVERIFIABLE_PREFIX_ASSIGN_VAR_0}' is set for one command that carries an expansion which can fail at runtime — whether the assignment stands for later commands cannot be statically verified
