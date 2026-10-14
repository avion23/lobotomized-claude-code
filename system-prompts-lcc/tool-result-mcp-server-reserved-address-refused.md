<!--
name: 'Tool Result: MCP server reserved address refused'
description: >-
  Explains Claude Code refuses an MCP server at an address it reserves and that
  retrying won't help
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_MCP_SERVER_RESERVED_ADDRESS_REFUSED_VAR_0
  - TOOL_RESULT_MCP_SERVER_RESERVED_ADDRESS_REFUSED_VAR_1
-->
Claude Code refuses MCP server "${TOOL_RESULT_MCP_SERVER_RESERVED_ADDRESS_REFUSED_VAR_0(TOOL_RESULT_MCP_SERVER_RESERVED_ADDRESS_REFUSED_VAR_1)}" because it reserves that address for its own use. No administrator set this. Retrying won't help, only removing it or changing its address.
