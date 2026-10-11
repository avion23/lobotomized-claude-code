<!--
name: 'Tool Result: artifact type — Artifact type ……… (…).'
description: 'Identity, optional tier and release header of an Artifact type description.'
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_TYPE_VAR_0
  - TOOL_RESULT_ARTIFACT_TYPE_VAR_1
  - TOOL_RESULT_ARTIFACT_TYPE_VAR_2
  - TOOL_RESULT_ARTIFACT_TYPE_VAR_3
  - TOOL_RESULT_ARTIFACT_TYPE_VAR_4
-->
Artifact type ${TOOL_RESULT_ARTIFACT_TYPE_VAR_0}${TOOL_RESULT_ARTIFACT_TYPE_VAR_1(TOOL_RESULT_ARTIFACT_TYPE_VAR_2.tier)?` [${TOOL_RESULT_ARTIFACT_TYPE_VAR_2.tier}]`:""}${typeof TOOL_RESULT_ARTIFACT_TYPE_VAR_2.release==="string"?`, release ${TOOL_RESULT_ARTIFACT_TYPE_VAR_3(TOOL_RESULT_ARTIFACT_TYPE_VAR_2.release)}`:""} (${TOOL_RESULT_ARTIFACT_TYPE_VAR_4}).
