<!--
name: 'Tool Result: MCP server handshake mismatch'
description: >-
  Deny when the MCP server no longer matches its start-up capabilities, name,
  version or instructions
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_MCP_SERVER_HANDSHAKE_MISMATCH_VAR_0
  - TOOL_RESULT_MCP_SERVER_HANDSHAKE_MISMATCH_VAR_1
-->
MCP server "${TOOL_RESULT_MCP_SERVER_HANDSHAKE_MISMATCH_VAR_0.name}" does not match what Claude Code was given at start-up (in its capabilities, name, version or instructions), so the call was not made. ${TOOL_RESULT_MCP_SERVER_HANDSHAKE_MISMATCH_VAR_1}
