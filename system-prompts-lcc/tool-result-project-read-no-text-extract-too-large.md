<!--
name: 'Tool Result: project_read no text extract and too large'
description: >-
  project_read refusal when a file has no text extract and is above the download
  limit.
ccVersion: 2.1.308
variables:
  - TOOL_RESULT_PROJECT_READ_NO_TEXT_EXTRACT_TOO_LARGE_VAR_0
  - TOOL_RESULT_PROJECT_READ_NO_TEXT_EXTRACT_TOO_LARGE_VAR_1
  - TOOL_RESULT_PROJECT_READ_NO_TEXT_EXTRACT_TOO_LARGE_VAR_2
-->
project_read: "${TOOL_RESULT_PROJECT_READ_NO_TEXT_EXTRACT_TOO_LARGE_VAR_0(TOOL_RESULT_PROJECT_READ_NO_TEXT_EXTRACT_TOO_LARGE_VAR_1)}" has no text extract and ${TOOL_RESULT_PROJECT_READ_NO_TEXT_EXTRACT_TOO_LARGE_VAR_2}; tell the user this file cannot be opened here.
