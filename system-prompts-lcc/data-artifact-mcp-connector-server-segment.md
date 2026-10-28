<!--
name: 'Data: Artifact MCP connector server segment'
description: >-
  Branch of the Artifact MCP connector guidance telling the model to take the
  server value from the mcp__<connector>__<tool> prefix segment, copied exactly,
  resolved to a display name at publish
ccVersion: 2.1.310
variables:
  - DATA_ARTIFACT_MCP_CONNECTOR_SERVER_SEGMENT_VAR_0
-->
Connector tools appear in your tool list as \`mcp__<connector>__<toolName>\`. Set \`server\` to the \`<connector>\` segment — everything between \`mcp__\` and the next \`__\` (for \`mcp__${DATA_ARTIFACT_MCP_CONNECTOR_SERVER_SEGMENT_VAR_0()}__search\`, the \`server\` is \`${DATA_ARTIFACT_MCP_CONNECTOR_SERVER_SEGMENT_VAR_0()}\`). Copy the segment exactly, case included; when publishing, it is resolved to the connector's display name automatically. In the page's own \`callTool\`/\`watchTool\` calls, pass the connector's display name (its name as shown in claude.ai), not that segment — viewers resolve connectors by name only. The publish result states the exact display name for each segment it resolves; if the page's calls do not match it, fix them and publish again.
