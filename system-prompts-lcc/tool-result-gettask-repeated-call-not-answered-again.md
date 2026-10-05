<!--
name: 'GetTask: repeated identical call not re-answered'
description: >-
  Error returned to the model when it calls GetTask on the same task and status
  combination more than the allowed number of times within one response.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_GETTASK_REPEATED_CALL_NOT_ANSWERED_AGAIN_VAR_0
  - TOOL_RESULT_GETTASK_REPEATED_CALL_NOT_ANSWERED_AGAIN_VAR_1
  - TOOL_RESULT_GETTASK_REPEATED_CALL_NOT_ANSWERED_AGAIN_VAR_2
-->
${TOOL_RESULT_GETTASK_REPEATED_CALL_NOT_ANSWERED_AGAIN_VAR_0} was already answered ${TOOL_RESULT_GETTASK_REPEATED_CALL_NOT_ANSWERED_AGAIN_VAR_1} times for this task in this response (status: ${TOOL_RESULT_GETTASK_REPEATED_CALL_NOT_ANSWERED_AGAIN_VAR_2}); the same call repeated within one response is not answered again.
