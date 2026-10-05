<!--
name: 'MCP passthrough: generic server error passthrough'
description: >-
  Wrapped error text for a passthrough MCP tool call that forwards the
  underlying server error's message, noting the call did not run.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_MCP_PASSTHROUGH_SERVER_GENERIC_ERROR_VAR_0
  - TOOL_RESULT_MCP_PASSTHROUGH_SERVER_GENERIC_ERROR_VAR_1
-->
MCP server "${TOOL_RESULT_MCP_PASSTHROUGH_SERVER_GENERIC_ERROR_VAR_0}" on this machine: ${TOOL_RESULT_MCP_PASSTHROUGH_SERVER_GENERIC_ERROR_VAR_1.message}; the call did not run
