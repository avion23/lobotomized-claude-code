<!--
name: 'Tool Result: MCP tool idle timeout'
description: >-
  MCP tool call error when the server sent no response or progress for longer
  than the idle timeout; explains the per-server timeout and
  CLAUDE_CODE_MCP_TOOL_IDLE_TIMEOUT.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_MCP_TOOL_IDLE_TIMEOUT_VAR_0
  - TOOL_RESULT_MCP_TOOL_IDLE_TIMEOUT_VAR_1
  - TOOL_RESULT_MCP_TOOL_IDLE_TIMEOUT_VAR_2
-->
MCP server "${TOOL_RESULT_MCP_TOOL_IDLE_TIMEOUT_VAR_0}" tool "${TOOL_RESULT_MCP_TOOL_IDLE_TIMEOUT_VAR_1}" sent no response or progress for ${TOOL_RESULT_MCP_TOOL_IDLE_TIMEOUT_VAR_2}s; aborting. If this server is configured in your MCP settings, set a per-server "timeout" (ms) to allow longer silent runs for just this server; otherwise set CLAUDE_CODE_MCP_TOOL_IDLE_TIMEOUT (ms) globally (0 disables).
