<!--
name: 'Tool Result: auto mode no verdict, call skipped'
description: >-
  Classifier gave no verdict because it expected the call not to need review;
  retry once, then tell the user.
ccVersion: 2.1.308
variables:
  - TOOL_RESULT_AUTO_MODE_NO_VERDICT_CALL_SKIPPED_VAR_0
  - TOOL_RESULT_AUTO_MODE_NO_VERDICT_CALL_SKIPPED_VAR_1
-->
${TOOL_RESULT_AUTO_MODE_NO_VERDICT_CALL_SKIPPED_VAR_0} gave no verdict for ${TOOL_RESULT_AUTO_MODE_NO_VERDICT_CALL_SKIPPED_VAR_1}: it expected this call not to need a review, but the call needed one. This is not a judgment that the action is unsafe. Issue the action again once, as-is; if it is denied again, do not issue it again: continue with other tasks that don't require it and tell the user that auto mode could not evaluate it. 
