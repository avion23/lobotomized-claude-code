<!--
name: 'Call status: awaiting session approval'
description: >-
  Tells the model a call is waiting on the target for the session's approval, so
  nothing has run yet.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_CALL_STATUS_AWAITING_APPROVAL_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_CALL_STATUS_AWAITING_APPROVAL_VAR_1
-->
This call is waiting on ${TOOL_RESULT_REMOTE_TOOL_CALL_STATUS_AWAITING_APPROVAL_VAR_0.name} for the session's approval (received ${TOOL_RESULT_REMOTE_TOOL_CALL_STATUS_AWAITING_APPROVAL_VAR_1} s ago); nothing has run yet.
