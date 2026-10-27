<!--
name: 'System Reminder: MCP failed servers reconnect by search'
description: Status clause that a ToolSearch query naming a failed server reconnects it
ccVersion: 2.1.311
variables:
  - SYSTEM_REMINDER_MCP_SERVERS_FAILED_TO_CONNECT_SEARCH_RECONNECTS_VAR_0
-->
for now; a ${SYSTEM_REMINDER_MCP_SERVERS_FAILED_TO_CONNECT_SEARCH_RECONNECTS_VAR_0} query that contains a server's name connects to it again, so once the server is running (for example after you start the app that serves it), search for its tools that way instead of reaching the server another way
