<!--
name: '/mcp: server pending approval'
description: >-
  /mcp action result when the named server is still pending approval, with an
  approve hint.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_MCP_RECONNECT_PENDING_APPROVAL_VAR_0
  - SLASH_COMMAND_MCP_RECONNECT_PENDING_APPROVAL_VAR_1
  - SLASH_COMMAND_MCP_RECONNECT_PENDING_APPROVAL_VAR_2
-->
"${SLASH_COMMAND_MCP_RECONNECT_PENDING_APPROVAL_VAR_0(SLASH_COMMAND_MCP_RECONNECT_PENDING_APPROVAL_VAR_1)}" is pending approval.${SLASH_COMMAND_MCP_RECONNECT_PENDING_APPROVAL_VAR_2(" Approve it with `/mcp` in the terminal first."," Open MCP servers from the command menu.")}
