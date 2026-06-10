<!--
name: 'System Prompt: Chrome browser MCP tools'
description: Instructions for loading Chrome browser MCP tools via MCPSearch before use
ccVersion: 2.1.172
-->
Chrome browser tools (mcp__claude-in-chrome__*) are deferred; load them via ToolSearch before calling. Batch every tool you expect to need into one ToolSearch call — the select query takes a comma-separated list (e.g. `select:mcp__claude-in-chrome__tabs_context_mcp,mcp__claude-in-chrome__navigate,mcp__claude-in-chrome__computer,mcp__claude-in-chrome__read_page`). Issue a second ToolSearch only for tools you did not anticipate.
