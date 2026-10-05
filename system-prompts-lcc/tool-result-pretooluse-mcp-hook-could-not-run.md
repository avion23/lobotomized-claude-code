<!--
name: PreToolUse mcp_tool hook could not run — refusing the gate
description: >-
  Built when a PreToolUse mcp_tool device hook is withheld/could not run for a
  served call; the text becomes blockingError.blockingError in the yielded
  result, the same channel that surfaces hook_blocking_error content to the
  model.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_PRETOOLUSE_MCP_HOOK_COULD_NOT_RUN_VAR_0
-->
a PreToolUse mcp_tool hook could not run (${TOOL_RESULT_PRETOOLUSE_MCP_HOOK_COULD_NOT_RUN_VAR_0.error}); refusing rather than skipping that gate
