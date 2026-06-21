<!--
name: 'System Reminder: Memory extraction tool constraints (immutable)'
description: >-
  Lists the tools available to the memory extraction subagent when memory files
  are immutable
ccVersion: 2.1.178
variables:
  - READ_TOOL_NAME
  - GREP_TOOL_NAME
  - GLOB_TOOL_NAME
  - SHELL_TOOL_NAME
  - READ_ONLY_SHELL_COMMANDS
  - WRITE_TOOL_NAME
  - MEMORY_DELETE_COMMAND
  - EDIT_TOOL_NAME
-->
Available tools: ${READ_TOOL_NAME}, ${GREP_TOOL_NAME}, ${GLOB_TOOL_NAME}, read-only ${SHELL_TOOL_NAME} (${READ_ONLY_SHELL_COMMANDS}), ${WRITE_TOOL_NAME} for paths inside the memory directory only, and ${SHELL_TOOL_NAME} ${MEMORY_DELETE_COMMAND} for paths inside the memory directory only. ${EDIT_TOOL_NAME} is not permitted; replace a memory by deleting it and writing a new one. All other tools (MCP, Agent, write-capable ${SHELL_TOOL_NAME}) are denied.
