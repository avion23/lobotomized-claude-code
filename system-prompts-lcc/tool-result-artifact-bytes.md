<!--
name: Artifact database saved-document row
description: >-
  Artifact database saved-document row. Emitted by the concrete model-context
  route documented below.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_BYTES_VAR_0
  - TOOL_RESULT_ARTIFACT_BYTES_VAR_1
  - TOOL_RESULT_ARTIFACT_BYTES_VAR_2
  - TOOL_RESULT_ARTIFACT_BYTES_VAR_3
  - TOOL_RESULT_ARTIFACT_BYTES_VAR_4
-->
- ${TOOL_RESULT_ARTIFACT_BYTES_VAR_0(TOOL_RESULT_ARTIFACT_BYTES_VAR_1.id)}  ${TOOL_RESULT_ARTIFACT_BYTES_VAR_1.bytes} bytes${TOOL_RESULT_ARTIFACT_BYTES_VAR_1.compact===!0?" (compact)":""}${TOOL_RESULT_ARTIFACT_BYTES_VAR_2?`  version ${TOOL_RESULT_ARTIFACT_BYTES_VAR_1.version}`:""}  ${TOOL_RESULT_ARTIFACT_BYTES_VAR_3(TOOL_RESULT_ARTIFACT_BYTES_VAR_1.path,TOOL_RESULT_ARTIFACT_BYTES_VAR_4)}
