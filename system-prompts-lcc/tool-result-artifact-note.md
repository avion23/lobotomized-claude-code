<!--
name: 'Artifact: Preview note'
description: >-
  Preview note. Text emitted in an Artifact tool result or tool validation
  error.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_NOTE_VAR_0
  - TOOL_RESULT_ARTIFACT_NOTE_VAR_1
-->
- note: ${TOOL_RESULT_ARTIFACT_NOTE_VAR_0(TOOL_RESULT_ARTIFACT_NOTE_VAR_1.text,1000)}
