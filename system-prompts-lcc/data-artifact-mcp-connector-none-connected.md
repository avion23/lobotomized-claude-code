<!--
name: Artifact MCP connector none connected
description: Note that no connectors are connected right now and how their tools appear
ccVersion: 2.1.310
variables:
  - DATA_ARTIFACT_MCP_CONNECTOR_NONE_CONNECTED_VAR_0
-->
None are connected right now — they may still be connecting, or the user has none. ${DATA_ARTIFACT_MCP_CONNECTOR_NONE_CONNECTED_VAR_0()?"When one connects, its tools appear in your tool list as `mcp__<connector>__<tool>`.":"Look for tools prefixed `mcp__claude_ai_*` in your tool list; each is named `mcp__claude_ai_<connector>__<tool>`."}
