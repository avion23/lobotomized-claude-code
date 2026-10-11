<!--
name: 'Claude Code skill: MCP server context'
description: Configured MCP server list in current-build context.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_CLAUDE_CODE_CURRENT_BUILD_MCP_SERVERS_VAR_0
-->
**Configured MCP servers:**
${SLASH_COMMAND_CLAUDE_CODE_CURRENT_BUILD_MCP_SERVERS_VAR_0.join(`
`)}
