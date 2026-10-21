<!--
name: 'Tool result: ReadCalls invalid tool_use_id'
description: ReadCalls served-tool error when a passed tool_use_id is not valid.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_READ_CALLS_INVALID_TOOL_USE_ID_VAR_0
  - TOOL_RESULT_READ_CALLS_INVALID_TOOL_USE_ID_VAR_1
  - TOOL_RESULT_READ_CALLS_INVALID_TOOL_USE_ID_VAR_2
-->
ReadCalls: ${TOOL_RESULT_READ_CALLS_INVALID_TOOL_USE_ID_VAR_0(TOOL_RESULT_READ_CALLS_INVALID_TOOL_USE_ID_VAR_1)} is not a valid tool_use_id${TOOL_RESULT_READ_CALLS_INVALID_TOOL_USE_ID_VAR_2.length>0?` (and ${TOOL_RESULT_READ_CALLS_INVALID_TOOL_USE_ID_VAR_2.length} more)`:""}. An id is 1 to 128 letters, digits or _ . : @ -, and not only dots.
