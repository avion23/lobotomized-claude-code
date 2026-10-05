<!--
name: 'Duplicate call, already answered'
description: >-
  Tells the model this request was already answered on the target and nothing
  further ran for it.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_REQUEST_ALREADY_ANSWERED_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_REQUEST_ALREADY_ANSWERED_VAR_1
  - TOOL_RESULT_REMOTE_TOOL_REQUEST_ALREADY_ANSWERED_VAR_2
-->
This request was already answered on ${TOOL_RESULT_REMOTE_TOOL_REQUEST_ALREADY_ANSWERED_VAR_0}: nothing was run for it (${TOOL_RESULT_REMOTE_TOOL_REQUEST_ALREADY_ANSWERED_VAR_1(TOOL_RESULT_REMOTE_TOOL_REQUEST_ALREADY_ANSWERED_VAR_2)}).
