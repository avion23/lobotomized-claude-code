<!--
name: 'Artifact publish: total content exceeds MB at a specific file'
description: >-
  Validation error identifying the specific file path at which cumulative
  publish content crosses the total-size cap.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_PUBLISH_FILES_TOTAL_CONTENT_EXCEEDS_MB_AT_PATH_VAR_0
  - TOOL_RESULT_ARTIFACT_PUBLISH_FILES_TOTAL_CONTENT_EXCEEDS_MB_AT_PATH_VAR_1
  - TOOL_RESULT_ARTIFACT_PUBLISH_FILES_TOTAL_CONTENT_EXCEEDS_MB_AT_PATH_VAR_2
  - TOOL_RESULT_ARTIFACT_PUBLISH_FILES_TOTAL_CONTENT_EXCEEDS_MB_AT_PATH_VAR_3
-->
files: total content exceeds ${TOOL_RESULT_ARTIFACT_PUBLISH_FILES_TOTAL_CONTENT_EXCEEDS_MB_AT_PATH_VAR_0/1024/1024}MB at ${TOOL_RESULT_ARTIFACT_PUBLISH_FILES_TOTAL_CONTENT_EXCEEDS_MB_AT_PATH_VAR_1.stringify(TOOL_RESULT_ARTIFACT_PUBLISH_FILES_TOTAL_CONTENT_EXCEEDS_MB_AT_PATH_VAR_2)} — the most one publish sends; publish the files up to it now and the rest in another publish to the same url (a version may total ${TOOL_RESULT_ARTIFACT_PUBLISH_FILES_TOTAL_CONTENT_EXCEEDS_MB_AT_PATH_VAR_3/1024/1024}MB)
