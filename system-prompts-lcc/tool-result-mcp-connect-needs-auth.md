<!--
name: 'MCP connect: needs authentication'
description: Lists MCP servers needing authentication and tells the user to run /mcp.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_MCP_CONNECT_NEEDS_AUTH_VAR_0
-->
Needs authentication (ask the user to run /mcp): ${TOOL_RESULT_MCP_CONNECT_NEEDS_AUTH_VAR_0.join(", ")}
