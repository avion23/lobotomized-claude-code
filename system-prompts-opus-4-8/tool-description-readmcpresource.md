<!--
name: 'Tool Description: ReadMCPResource'
description: Tool description for reading a specific MCP server resource by URI
ccVersion: 2.1.185
variables:
  - TOOL_DESCRIPTION_READMCPRESOURCE_VAR_0
-->

Reads a specific resource from an MCP server, identified by server name and resource URI.

Parameters:
- server (required): The name of the MCP server from which to read the resource
- uri (required): The URI of the resource to read

When the URI names a directory resource on a server that supports directory listing, the result carries a "resources" array listing the directory's direct children. Subdirectories appear with mimeType "${TOOL_DESCRIPTION_READMCPRESOURCE_VAR_0}"; read them again to descend.
