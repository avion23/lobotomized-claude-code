<!--
name: WebFetch artifact refused fallback clause
description: >-
  Clause telling Claude which tool to use where the Artifacts MCP read tool
  refuses a link
ccVersion: 2.1.310
variables:
  - TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_REFUSED_USE_FALLBACK_VAR_0
  - TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_REFUSED_USE_FALLBACK_VAR_1
-->
 Where it refuses one, use ${TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_REFUSED_USE_FALLBACK_VAR_0}, not ${TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_REFUSED_USE_FALLBACK_VAR_1}.
