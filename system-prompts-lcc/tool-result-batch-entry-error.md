<!--
name: 'Batched tool: entry error'
description: Batched tool result line for an entry that errored or returned nothing
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BATCH_ENTRY_ERROR_VAR_0
  - TOOL_RESULT_BATCH_ENTRY_ERROR_VAR_1
-->
[entry ${TOOL_RESULT_BATCH_ENTRY_ERROR_VAR_0+1} error: ${TOOL_RESULT_BATCH_ENTRY_ERROR_VAR_1.error??"no result"}]
