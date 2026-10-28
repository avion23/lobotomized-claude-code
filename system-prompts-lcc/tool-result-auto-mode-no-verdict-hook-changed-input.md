<!--
name: 'Tool Result: No verdict — hook changed input after review'
description: >-
  Wrapper deny message when a hook changed the call's input after auto mode
  reviewed it, so the review does not cover what would run
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AUTO_MODE_NO_VERDICT_HOOK_CHANGED_INPUT_VAR_0
  - TOOL_RESULT_AUTO_MODE_NO_VERDICT_HOOK_CHANGED_INPUT_VAR_1
  - TOOL_RESULT_AUTO_MODE_NO_VERDICT_HOOK_CHANGED_INPUT_VAR_2
-->
${TOOL_RESULT_AUTO_MODE_NO_VERDICT_HOOK_CHANGED_INPUT_VAR_0} gave no verdict for ${TOOL_RESULT_AUTO_MODE_NO_VERDICT_HOOK_CHANGED_INPUT_VAR_1}: a hook changed this call's input after auto mode reviewed it, so the review does not cover what would run. This is not a judgment that the action is unsafe. ${TOOL_RESULT_AUTO_MODE_NO_VERDICT_HOOK_CHANGED_INPUT_VAR_2} 
