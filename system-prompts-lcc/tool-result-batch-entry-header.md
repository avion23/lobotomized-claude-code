<!--
name: 'Batched tool: entry header'
description: Batched tool result separator line naming the entry and whether it errored
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BATCH_ENTRY_HEADER_VAR_0
  - TOOL_RESULT_BATCH_ENTRY_HEADER_VAR_1
-->
--- entry ${TOOL_RESULT_BATCH_ENTRY_HEADER_VAR_0+1}${TOOL_RESULT_BATCH_ENTRY_HEADER_VAR_1?" (error)":""} ---
