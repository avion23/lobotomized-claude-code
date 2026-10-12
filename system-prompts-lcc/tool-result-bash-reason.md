<!--
name: 'Tool Result: bash coordinator — Reason: ….'
description: Bash refusal reason copied from its read-only analysis.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_REASON_VAR_0
  - TOOL_RESULT_BASH_REASON_VAR_1
  - TOOL_RESULT_BASH_REASON_VAR_2
-->
Reason: ${TOOL_RESULT_BASH_REASON_VAR_0(TOOL_RESULT_BASH_REASON_VAR_1.message.replace(/\.$/,""),TOOL_RESULT_BASH_REASON_VAR_2)}.
