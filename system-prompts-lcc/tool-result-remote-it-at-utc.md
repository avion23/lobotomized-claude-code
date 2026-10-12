<!--
name: Remote duplicate call completed
description: >-
  Remote duplicate call completed. Emitted by the concrete model-context route
  documented below.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_REMOTE_IT_AT_UTC_VAR_0
  - TOOL_RESULT_REMOTE_IT_AT_UTC_VAR_1
-->
it ${TOOL_RESULT_REMOTE_IT_AT_UTC_VAR_0.isError?"completed with an error":"completed"} at ${TOOL_RESULT_REMOTE_IT_AT_UTC_VAR_1} UTC
