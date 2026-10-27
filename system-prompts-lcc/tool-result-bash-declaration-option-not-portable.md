<!--
name: 'Tool Result: Bash declaration option not portable'
description: >-
  Ask reason when a declaration option is not known to be accepted by both bash
  and zsh
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_BASH_DECLARATION_OPTION_NOT_PORTABLE_VAR_0
  - TOOL_RESULT_BASH_DECLARATION_OPTION_NOT_PORTABLE_VAR_1
  - TOOL_RESULT_BASH_DECLARATION_OPTION_NOT_PORTABLE_VAR_2
-->
${TOOL_RESULT_BASH_DECLARATION_OPTION_NOT_PORTABLE_VAR_0} option '${TOOL_RESULT_BASH_DECLARATION_OPTION_NOT_PORTABLE_VAR_1(TOOL_RESULT_BASH_DECLARATION_OPTION_NOT_PORTABLE_VAR_2)}' is not one bash and zsh are both known to accept — a shell that rejects it assigns nothing, so the names it declares cannot be statically verified
