<!--
name: 'Tool Result: ToolSearch MCP servers reserved address'
description: >-
  ToolSearch note that Claude Code refuses configured MCP servers whose address
  it reserves, so retrying will not help
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_TOOLSEARCH_MCP_SERVERS_RESERVED_ADDRESS_VAR_0
  - TOOL_RESULT_TOOLSEARCH_MCP_SERVERS_RESERVED_ADDRESS_VAR_1
  - TOOL_RESULT_TOOLSEARCH_MCP_SERVERS_RESERVED_ADDRESS_VAR_2
-->
${TOOL_RESULT_TOOLSEARCH_MCP_SERVERS_RESERVED_ADDRESS_VAR_0.endsWith(".")?"":"."} Note: Claude Code itself refuses these configured MCP servers because it reserves their address for its own use, so their tools are unavailable: ${TOOL_RESULT_TOOLSEARCH_MCP_SERVERS_RESERVED_ADDRESS_VAR_1}${TOOL_RESULT_TOOLSEARCH_MCP_SERVERS_RESERVED_ADDRESS_VAR_2}. This is not a connection failure or an administrator's setting, so retrying will not help; whoever added the entry can remove it or change its address.
