<!--
name: 'More saved documents (named list, Artifact DB)'
description: >-
  Continuation fragment listing additional saved documents by id when they fit
  within the result budget.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_DB_READ_SAVED_MORE_NAMED_VAR_0
  - TOOL_RESULT_ARTIFACT_DB_READ_SAVED_MORE_NAMED_VAR_1
  - TOOL_RESULT_ARTIFACT_DB_READ_SAVED_MORE_NAMED_VAR_2
-->

[${TOOL_RESULT_ARTIFACT_DB_READ_SAVED_MORE_NAMED_VAR_0} more saved ${TOOL_RESULT_ARTIFACT_DB_READ_SAVED_MORE_NAMED_VAR_1(TOOL_RESULT_ARTIFACT_DB_READ_SAVED_MORE_NAMED_VAR_0,"document")}, at <that directory>/<doc_id>.json each${TOOL_RESULT_ARTIFACT_DB_READ_SAVED_MORE_NAMED_VAR_2?" (id, version)":""}: 
