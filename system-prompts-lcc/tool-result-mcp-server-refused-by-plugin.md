<!--
name: 'Tool result: MCP server refused by plugin'
description: >-
  MCP tool error when the providing plugin refused the call; says to retry once
  and treat a second refusal as the server being off.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_MCP_SERVER_REFUSED_BY_PLUGIN_VAR_0
-->
MCP server "${TOOL_RESULT_MCP_SERVER_REFUSED_BY_PLUGIN_VAR_0}" was not called: the plugin that provides it refused this call. Try the call once more. If it is refused again, the plugin has turned the server off.
