<!--
name: 'Artifact: Viewer console message'
description: >-
  Viewer console message. Text emitted in an Artifact tool result or tool
  validation error.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_CONSOLE_VAR_0
  - TOOL_RESULT_ARTIFACT_CONSOLE_VAR_1
-->
- console: ${TOOL_RESULT_ARTIFACT_CONSOLE_VAR_0(TOOL_RESULT_ARTIFACT_CONSOLE_VAR_1,1000)}
