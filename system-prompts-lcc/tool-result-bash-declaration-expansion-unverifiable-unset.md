<!--
name: 'Bash: unset behind a failable expansion unverifiable'
description: >-
  Permission reason when an unset rides a command whose expansion can fail at
  runtime
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_DECLARATION_EXPANSION_UNVERIFIABLE_UNSET_VAR_0
-->
'unset ${TOOL_RESULT_BASH_DECLARATION_EXPANSION_UNVERIFIABLE_UNSET_VAR_0}' is in a command carrying an expansion that can fail at runtime — whether the name is cleared cannot be statically verified
