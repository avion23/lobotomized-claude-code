<!--
name: '/mcp: server already in state'
description: >-
  /mcp enable|disable result when the named server is already enabled or
  disabled.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_MCP_TOGGLE_SERVER_ALREADY_IN_STATE_VAR_0
  - SLASH_COMMAND_MCP_TOGGLE_SERVER_ALREADY_IN_STATE_VAR_1
  - SLASH_COMMAND_MCP_TOGGLE_SERVER_ALREADY_IN_STATE_VAR_2
-->
"${SLASH_COMMAND_MCP_TOGGLE_SERVER_ALREADY_IN_STATE_VAR_0(SLASH_COMMAND_MCP_TOGGLE_SERVER_ALREADY_IN_STATE_VAR_1)}" is already ${SLASH_COMMAND_MCP_TOGGLE_SERVER_ALREADY_IN_STATE_VAR_2?"enabled":"disabled"}.
