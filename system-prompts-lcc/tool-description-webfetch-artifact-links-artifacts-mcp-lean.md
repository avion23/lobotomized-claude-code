<!--
name: WebFetch artifact links via Artifacts MCP (lean)
description: >-
  Lean WebFetch prompt clause that claude.ai artifact links should be read with
  the Artifacts MCP read tool
ccVersion: 2.1.310
variables:
  - TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_LINKS_ARTIFACTS_MCP_LEAN_VAR_0
  - TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_LINKS_ARTIFACTS_MCP_LEAN_VAR_1
-->
 claude.ai artifact links (claude.ai/artifact/{id} or claude.ai/code/artifact/{uuid}) are published artifacts: read them with ${TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_LINKS_ARTIFACTS_MCP_LEAN_VAR_0()}, which takes the link.${TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_LINKS_ARTIFACTS_MCP_LEAN_VAR_1("curl")}
