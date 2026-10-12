<!--
name: 'Tool Result: artifact file contentType prefix'
description: >-
  Head fragment of the artifact files-validator refusals naming the file and its
  contentType, followed by 'is binary…' or 'is a text type but the Buffer is not
  valid UTF-8…'.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_FILE_CONTENT_TYPE_PREFIX_VAR_0
  - TOOL_RESULT_ARTIFACT_FILE_CONTENT_TYPE_PREFIX_VAR_1
-->
file ${TOOL_RESULT_ARTIFACT_FILE_CONTENT_TYPE_PREFIX_VAR_0(TOOL_RESULT_ARTIFACT_FILE_CONTENT_TYPE_PREFIX_VAR_1.path)}: contentType ${TOOL_RESULT_ARTIFACT_FILE_CONTENT_TYPE_PREFIX_VAR_0(TOOL_RESULT_ARTIFACT_FILE_CONTENT_TYPE_PREFIX_VAR_1.contentType)} 
