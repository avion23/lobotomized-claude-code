<!--
name: 'Tool Result: MCP wait for servers failed'
description: WaitForMcpServers tool_result line listing servers that failed to connect.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_MCP_WAIT_FOR_SERVERS_FAILED_VAR_0
-->
Failed to connect: ${TOOL_RESULT_MCP_WAIT_FOR_SERVERS_FAILED_VAR_0.failed.join(", ")}
