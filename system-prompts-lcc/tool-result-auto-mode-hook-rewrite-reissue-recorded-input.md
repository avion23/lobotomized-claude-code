<!--
name: 'Tool Result: Reissue hook-rewritten call as recorded'
description: >-
  Clause telling Claude to issue the call once more exactly as the conversation
  records it so auto mode reviews it
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_RECORDED_INPUT_VAR_0
  - TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_RECORDED_INPUT_VAR_1
  - TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_RECORDED_INPUT_VAR_2
-->
${TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_RECORDED_INPUT_VAR_0.kind==="too_long"?"The input is too long to quote here. ":""}Issue the ${TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_RECORDED_INPUT_VAR_1} call once more exactly as this conversation records it so auto mode reviews it. If it is denied again, do not retry; ${TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_RECORDED_INPUT_VAR_2}
