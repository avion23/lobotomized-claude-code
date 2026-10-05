<!--
name: 'MCP passthrough: server returned an error'
description: >-
  Wrapped error text for a passthrough MCP tool call reporting the local MCP
  server returned an error for the call, noting it may have had effects.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_MCP_PASSTHROUGH_SERVER_RETURNED_ERROR_VAR_0
  - TOOL_RESULT_MCP_PASSTHROUGH_SERVER_RETURNED_ERROR_VAR_1
-->
MCP server "${TOOL_RESULT_MCP_PASSTHROUGH_SERVER_RETURNED_ERROR_VAR_0}" on this machine returned an error for the call (it reached the server and may have had effects): ${TOOL_RESULT_MCP_PASSTHROUGH_SERVER_RETURNED_ERROR_VAR_1.message}
