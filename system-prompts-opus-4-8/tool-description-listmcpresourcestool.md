<!--
name: 'Tool Description: ListMcpResourcesTool'
description: >-
  Tool description for listing available MCP resources from all configured
  servers or a specific server
ccVersion: 2.1.178
-->

Lists available resources from configured MCP servers. Each resource includes a 'server' field indicating which server it's from.

Pass `server` to list resources from one server (e.g. `listMcpResources({ server: "myserver" })`); omit it to list from all.
