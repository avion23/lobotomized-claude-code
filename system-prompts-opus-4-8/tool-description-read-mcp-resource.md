<!--
name: 'Tool Description: Read MCP Resource'
description: descriptionForModel for the ReadMcpResource tool.
ccVersion: 2.1.183
variables:
  - TOOL_DESCRIPTION_READ_MCP_RESOURCE_VAR_0
-->

Reads a specific resource from an MCP server, identified by server name and resource URI. Required params: `server` (the MCP server name) and `uri` (the resource URI).

When the URI names a directory resource on a server that supports directory listing, the result carries a "resources" array listing the directory's direct children. Subdirectories appear with mimeType "${TOOL_DESCRIPTION_READ_MCP_RESOURCE_VAR_0}"; read them again to descend.
