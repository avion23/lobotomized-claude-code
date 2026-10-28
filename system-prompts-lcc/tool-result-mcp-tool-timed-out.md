<!--
name: 'Tool Result: MCP tool timed out'
description: >-
  MCP tool error when a call exceeded the tool timeout, optionally followed by
  notes on open questions or pending state.
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_MCP_TOOL_TIMED_OUT_VAR_0
  - TOOL_RESULT_MCP_TOOL_TIMED_OUT_VAR_1
  - TOOL_RESULT_MCP_TOOL_TIMED_OUT_VAR_2
  - TOOL_RESULT_MCP_TOOL_TIMED_OUT_VAR_3
-->
MCP server "${TOOL_RESULT_MCP_TOOL_TIMED_OUT_VAR_0}" tool "${TOOL_RESULT_MCP_TOOL_TIMED_OUT_VAR_1}" timed out after ${TOOL_RESULT_MCP_TOOL_TIMED_OUT_VAR_2.floor(TOOL_RESULT_MCP_TOOL_TIMED_OUT_VAR_3/1000)}s
