<!--
name: 'Tool Result: artifact type — Title: …'
description: 'Artifact type title, with an Untitled fallback.'
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_TITLE_VAR_0
  - TOOL_RESULT_ARTIFACT_TITLE_VAR_1
-->
Title: ${TOOL_RESULT_ARTIFACT_TITLE_VAR_0(TOOL_RESULT_ARTIFACT_TITLE_VAR_1.title)??"Untitled"}
