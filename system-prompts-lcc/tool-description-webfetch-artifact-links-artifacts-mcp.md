<!--
name: WebFetch artifact links via Artifacts MCP
description: >-
  WebFetch prompt bullet that claude.ai artifact links should be read with the
  Artifacts MCP read tool, not curl or a headless browser
ccVersion: 2.1.310
variables:
  - TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_LINKS_ARTIFACTS_MCP_VAR_0
  - TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_LINKS_ARTIFACTS_MCP_VAR_1
-->
- claude.ai artifact links (claude.ai/artifact/{id} or claude.ai/code/artifact/{uuid}, including preview.claude.ai) are published artifacts: read them with ${TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_LINKS_ARTIFACTS_MCP_VAR_0()}, which takes the link.${TOOL_DESCRIPTION_WEBFETCH_ARTIFACT_LINKS_ARTIFACTS_MCP_VAR_1("curl or a headless browser")}
