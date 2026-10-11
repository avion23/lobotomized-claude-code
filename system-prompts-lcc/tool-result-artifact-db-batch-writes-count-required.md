<!--
name: 'Tool result: artifact db batch writes count required'
description: Batch write error when writes is empty or exceeds the entry cap.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_DB_BATCH_WRITES_COUNT_REQUIRED_VAR_0
  - TOOL_RESULT_ARTIFACT_DB_BATCH_WRITES_COUNT_REQUIRED_VAR_1
-->
db_op "${TOOL_RESULT_ARTIFACT_DB_BATCH_WRITES_COUNT_REQUIRED_VAR_0}" requires \`writes\` with 1-${TOOL_RESULT_ARTIFACT_DB_BATCH_WRITES_COUNT_REQUIRED_VAR_1} entries
