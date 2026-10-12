<!--
name: 'Artifact: Viewer marks'
description: >-
  Viewer marks. Text emitted in an Artifact tool result or tool validation
  error.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_VIEWER_MARKS_VAR_0
  - TOOL_RESULT_ARTIFACT_VIEWER_MARKS_VAR_1
-->
- viewer marks: ${TOOL_RESULT_ARTIFACT_VIEWER_MARKS_VAR_0(TOOL_RESULT_ARTIFACT_VIEWER_MARKS_VAR_1.marks.join(", "),1000)}
