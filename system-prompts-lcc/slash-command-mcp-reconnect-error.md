<!--
name: 'Slash Command: /mcp — reconnect error'
description: >-
  Bare "Error: <detail>" line. /mcp reconnect returns it with the sanitized
  error when reconnecting a server threw. The same generic template appears at
  other sites.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_MCP_RECONNECT_ERROR_VAR_0
  - SLASH_COMMAND_MCP_RECONNECT_ERROR_VAR_1
-->
Error: ${SLASH_COMMAND_MCP_RECONNECT_ERROR_VAR_0(SLASH_COMMAND_MCP_RECONNECT_ERROR_VAR_1)}
