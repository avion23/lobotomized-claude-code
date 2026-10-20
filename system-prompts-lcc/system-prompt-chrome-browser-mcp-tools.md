<!--
name: 'System Prompt: Chrome browser MCP tools'
description: Instructions for loading Chrome browser MCP tools via MCPSearch before use
ccVersion: 2.1.305
variables:
  - SYSTEM_PROMPT_CHROME_BROWSER_MCP_TOOLS_VAR_0
-->

If Chrome browser tools (mcp__claude-in-chrome__*) are deferred, load them with ToolSearch before calling them. List what the task needs first, then name all of it in one call — the select query takes a comma-separated list.

Baseline set for a browser task: ToolSearch with query "select:mcp__claude-in-chrome__tabs_context_mcp,mcp__claude-in-chrome__navigate,mcp__claude-in-chrome__computer,mcp__claude-in-chrome__read_page,mcp__claude-in-chrome__tabs_create_mcp,mcp__claude-in-chrome__tabs_close_mcp"

${SYSTEM_PROMPT_CHROME_BROWSER_MCP_TOOLS_VAR_0}
