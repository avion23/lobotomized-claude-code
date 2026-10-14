<!--
name: 'Tool Result: Artifact published but file lags'
description: >-
  Lead clause saying the page or artifact has the edits but the local file does
  not
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_ARTIFACT_EDITS_PUBLISHED_FILE_LAGS_VAR_0
  - TOOL_RESULT_ARTIFACT_EDITS_PUBLISHED_FILE_LAGS_VAR_1
  - TOOL_RESULT_ARTIFACT_EDITS_PUBLISHED_FILE_LAGS_VAR_2
-->
Published — ${TOOL_RESULT_ARTIFACT_EDITS_PUBLISHED_FILE_LAGS_VAR_0==="page"?"the page":"the artifact"} now has ${TOOL_RESULT_ARTIFACT_EDITS_PUBLISHED_FILE_LAGS_VAR_1?"the edit":`the ${TOOL_RESULT_ARTIFACT_EDITS_PUBLISHED_FILE_LAGS_VAR_2} edits`}, but the file at file_path does not
