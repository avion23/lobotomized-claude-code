<!--
name: 'Tool Result: MCP task malformed handle'
description: >-
  Says the MCP server returned a malformed task handle and the server may still
  run it
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_MCP_TASK_MALFORMED_HANDLE_VAR_0
  - TOOL_RESULT_MCP_TASK_MALFORMED_HANDLE_VAR_1
  - TOOL_RESULT_MCP_TASK_MALFORMED_HANDLE_VAR_2
-->
MCP server "${TOOL_RESULT_MCP_TASK_MALFORMED_HANDLE_VAR_0}" returned a malformed task handle for tool "${TOOL_RESULT_MCP_TASK_MALFORMED_HANDLE_VAR_1}", so Claude Code cannot track the task or get its result. ${TOOL_RESULT_MCP_TASK_MALFORMED_HANDLE_VAR_2.success?"It tried to cancel the task, but the":"The"} server may still be running it. Calling the tool again may start another task.
