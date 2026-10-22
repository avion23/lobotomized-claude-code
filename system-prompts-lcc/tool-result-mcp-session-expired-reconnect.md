<!--
name: 'Tool Result: MCP session expired, reconnect'
description: >-
  Tells the model the MCP session expired/connection closed; send mcp_reconnect
  and retry, with detail.
ccVersion: 2.1.308
variables:
  - TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_0
  - TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_1
  - TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_2
  - TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_3
  - TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_4
-->
${TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_0.mayHaveRun?`MCP connection to ${TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_1} closed during the call — send mcp_reconnect, and check whether the tool ran before retrying${TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_2}`:`MCP ${TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_0.expiryKind==="connection_closed_call_not_run"?"connection closed before the call ran on":"session expired for"} ${TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_1} — send mcp_reconnect and retry${TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_2}`}: ${TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_3(TOOL_RESULT_MCP_SESSION_EXPIRED_RECONNECT_VAR_4)}
