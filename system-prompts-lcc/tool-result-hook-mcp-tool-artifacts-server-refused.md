<!--
name: Hook mcp_tool Artifacts server refused
description: Hook error that hooks cannot call Artifacts MCP server tools
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_HOOK_MCP_TOOL_ARTIFACTS_SERVER_REFUSED_VAR_0
-->
Hooks can't call tools of MCP server '${TOOL_RESULT_HOOK_MCP_TOOL_ARTIFACTS_SERVER_REFUSED_VAR_0}' (the Artifacts MCP server), because a hook's call skips your permission rules. Remove this mcp_tool hook or point it at another server.
