<!--
name: Artifact Unresolved Connector Guidance
description: >-
  Model-facing tool_result fragment telling the model how to set the `server`
  segment for an unresolved MCP connector when an artifact's MCP manifest is
  rejected.
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_ARTIFACT_UNRESOLVED_CONNECTOR_GUIDANCE_VAR_0
-->
set \`server\` to the segment between \`mcp__\` and the next \`__\` of a tool name from this session (for \`mcp__${TOOL_RESULT_ARTIFACT_UNRESOLVED_CONNECTOR_GUIDANCE_VAR_0()}__search\`, use \`${TOOL_RESULT_ARTIFACT_UNRESOLVED_CONNECTOR_GUIDANCE_VAR_0()}\`, copied exactly), or to the connector's exact display name
