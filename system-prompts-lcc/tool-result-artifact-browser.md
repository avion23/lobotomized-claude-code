<!--
name: 'Artifact: Preview browser error'
description: >-
  Preview browser error. Text emitted in an Artifact tool result or tool
  validation error.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_BROWSER_VAR_0
  - TOOL_RESULT_ARTIFACT_BROWSER_VAR_1
-->
- browser: ${TOOL_RESULT_ARTIFACT_BROWSER_VAR_0(TOOL_RESULT_ARTIFACT_BROWSER_VAR_1.renderError,200)}
