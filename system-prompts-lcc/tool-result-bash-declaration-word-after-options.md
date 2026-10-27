<!--
name: 'Tool Result: Bash declaration word after options'
description: >-
  Ask reason when a declaration word follows the options and shells diverge on
  the resulting error
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_BASH_DECLARATION_WORD_AFTER_OPTIONS_VAR_0
  - TOOL_RESULT_BASH_DECLARATION_WORD_AFTER_OPTIONS_VAR_1
  - TOOL_RESULT_BASH_DECLARATION_WORD_AFTER_OPTIONS_VAR_2
-->
${TOOL_RESULT_BASH_DECLARATION_WORD_AFTER_OPTIONS_VAR_0} word '${TOOL_RESULT_BASH_DECLARATION_WORD_AFTER_OPTIONS_VAR_1(TOOL_RESULT_BASH_DECLARATION_WORD_AFTER_OPTIONS_VAR_2)}' comes after the options — the shell reads it as a name, which it cannot be, and bash and zsh go on from that error differently
