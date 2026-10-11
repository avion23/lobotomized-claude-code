<!--
name: Asset call failed — unsupported type
description: >-
  Artifact asset error arm for an unsupported_type code, defaulting to the list
  of file types the asset store accepts.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_ASSET_UNSUPPORTED_TYPE_VAR_0
  - TOOL_RESULT_ARTIFACT_ASSET_UNSUPPORTED_TYPE_VAR_1
  - TOOL_RESULT_ARTIFACT_ASSET_UNSUPPORTED_TYPE_VAR_2
-->
${TOOL_RESULT_ARTIFACT_ASSET_UNSUPPORTED_TYPE_VAR_0}: ${TOOL_RESULT_ARTIFACT_ASSET_UNSUPPORTED_TYPE_VAR_1??`only these file types are accepted: ${TOOL_RESULT_ARTIFACT_ASSET_UNSUPPORTED_TYPE_VAR_2}`}
