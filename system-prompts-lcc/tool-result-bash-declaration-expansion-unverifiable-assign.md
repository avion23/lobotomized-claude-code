<!--
name: Bash declaration expansion can fail
description: >-
  Ask reason that a variable assigned by a declaration with a failing expansion
  cannot be statically verified
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_DECLARATION_EXPANSION_UNVERIFIABLE_ASSIGN_VAR_0
-->
'${TOOL_RESULT_BASH_DECLARATION_EXPANSION_UNVERIFIABLE_ASSIGN_VAR_0}' is assigned by a declaration carrying an expansion that can fail at runtime, which assigns nothing when it fails — its value cannot be statically verified
