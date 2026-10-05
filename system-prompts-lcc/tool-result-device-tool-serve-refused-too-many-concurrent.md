<!--
name: 'Device tool refused: too many concurrent calls'
description: >-
  Refusal message for a served device-tool call explaining too many concurrent
  device-tool calls are open on this device connection, with the concurrency
  limit and instruction to retry after one finishes.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_TOO_MANY_CONCURRENT_VAR_0
  - TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_TOO_MANY_CONCURRENT_VAR_1
-->
${TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_TOO_MANY_CONCURRENT_VAR_0} refused: too many concurrent device tool calls on this device connection (limit ${TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_TOO_MANY_CONCURRENT_VAR_1.limit}); retry after one finishes.
