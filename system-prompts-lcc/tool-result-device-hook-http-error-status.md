<!--
name: 'Tool Result: Device HTTP Hook — endpoint answered with an HTTP error'
description: >-
  Tells the model that an HTTP hook did not run because its endpoint answered
  with an HTTP error status.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_DEVICE_HOOK_HTTP_ERROR_STATUS_VAR_0
-->
it answered HTTP ${TOOL_RESULT_DEVICE_HOOK_HTTP_ERROR_STATUS_VAR_0.statusCode??"with an error"}
