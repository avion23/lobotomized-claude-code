<!--
name: 'Tool Result: MCP wait for servers still connecting'
description: >-
  WaitForMcpServers tool_result line listing servers still connecting, telling
  the model to retry or proceed without them.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_MCP_WAIT_FOR_SERVERS_STILL_CONNECTING_VAR_0
-->
Still connecting (try again or proceed without): ${TOOL_RESULT_MCP_WAIT_FOR_SERVERS_STILL_CONNECTING_VAR_0.stillPending.join(", ")}
