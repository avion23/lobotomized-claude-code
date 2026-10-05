<!--
name: 'Call status: timed out or cancelled'
description: >-
  Fragment describing that a call ended timed-out or cancelled at a given time,
  so it may have partially run if it had started.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_CALL_STATUS_TIMED_OUT_OR_CANCELLED_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_CALL_STATUS_TIMED_OUT_OR_CANCELLED_VAR_1
-->
it ended as ${TOOL_RESULT_REMOTE_TOOL_CALL_STATUS_TIMED_OUT_OR_CANCELLED_VAR_0.code} at ${TOOL_RESULT_REMOTE_TOOL_CALL_STATUS_TIMED_OUT_OR_CANCELLED_VAR_1} UTC; if it had started, it may have partially run
