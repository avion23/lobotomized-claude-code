<!--
name: 'Tool Result: Artifacts MCP tools unavailable'
description: >-
  Deny message that the Artifact tool isn't available, so the Artifacts MCP
  tools aren't either, with a /login and /config hint on a laptop
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_ARTIFACT_MCP_ARTIFACT_TOOL_UNAVAILABLE_VAR_0
-->
The Artifact tool isn't available in this session, so the Artifacts MCP tools aren't available either.${TOOL_RESULT_ARTIFACT_MCP_ARTIFACT_TOOL_UNAVAILABLE_VAR_0==="laptop"?" Check /login and /config.":""}
