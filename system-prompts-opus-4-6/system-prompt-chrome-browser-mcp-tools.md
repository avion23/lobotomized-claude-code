<!--
name: 'System Prompt: Chrome browser MCP tools'
description: Instructions for loading Chrome browser MCP tools via MCPSearch before use
ccVersion: 2.1.172
-->
If Chrome browser tools (mcp__claude-in-chrome__*) are deferred, load them with ToolSearch before calling them. Batch every tool you'll need into one call — `select:` takes a comma-separated list — rather than one round-trip per tool.
