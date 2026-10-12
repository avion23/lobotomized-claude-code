<!--
name: 'Tool Result: MCP wait for servers connected'
description: >-
  WaitForMcpServers tool_result line listing servers that connected, telling the
  model to call their tools directly.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_MCP_WAIT_FOR_SERVERS_CONNECTED_VAR_0
-->
Connected (their tools are now available — call them directly): ${TOOL_RESULT_MCP_WAIT_FOR_SERVERS_CONNECTED_VAR_0.connected.join(", ")}
