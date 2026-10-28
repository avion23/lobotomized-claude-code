<!--
name: 'Tool Result: Hook-changed input cannot be quoted'
description: >-
  Clause when the hook-changed input is too long or cannot be written out, so
  the call cannot be issued in a reviewable form
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_INPUT_NOT_QUOTABLE_VAR_0
  - TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_INPUT_NOT_QUOTABLE_VAR_1
-->
${TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_INPUT_NOT_QUOTABLE_VAR_0.kind==="too_long"?"The changed input is too long to quote here":"The changed input cannot be written out here"}, so this call cannot be issued in a form auto mode can review; ${TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_INPUT_NOT_QUOTABLE_VAR_1}
