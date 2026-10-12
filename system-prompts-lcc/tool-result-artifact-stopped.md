<!--
name: 'Artifact: Viewer stop detail'
description: >-
  Viewer stop detail. Text emitted in an Artifact tool result or tool validation
  error.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_STOPPED_VAR_0
  - TOOL_RESULT_ARTIFACT_STOPPED_VAR_1
-->
- stopped: ${TOOL_RESULT_ARTIFACT_STOPPED_VAR_0(TOOL_RESULT_ARTIFACT_STOPPED_VAR_1,500)}
