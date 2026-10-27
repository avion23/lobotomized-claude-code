<!--
name: 'Bash: append behind a failable expansion unverifiable'
description: >-
  Permission reason when a variable append rides a command whose expansion can
  fail at runtime
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_DECLARATION_EXPANSION_UNVERIFIABLE_APPEND_VAR_0
-->
'${TOOL_RESULT_BASH_DECLARATION_EXPANSION_UNVERIFIABLE_APPEND_VAR_0.name}' is appended to by a command carrying an expansion that can fail at runtime — whether the append happens cannot be statically verified
