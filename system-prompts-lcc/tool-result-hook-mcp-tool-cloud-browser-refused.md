<!--
name: Hook mcp_tool cloud browser refused
description: Hook error that hooks cannot call cloud browser MCP tools
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_HOOK_MCP_TOOL_CLOUD_BROWSER_REFUSED_VAR_0
-->
Hooks can't call tools of MCP server '${TOOL_RESULT_HOOK_MCP_TOOL_CLOUD_BROWSER_REFUSED_VAR_0}' (the cloud browser) in this session, because a hook's call skips auto mode's safety check and your approval. Remove this mcp_tool hook or point it at another server.
