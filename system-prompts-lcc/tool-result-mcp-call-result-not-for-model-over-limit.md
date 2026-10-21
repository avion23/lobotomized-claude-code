<!--
name: 'Tool Result: mcp_call result over limit'
description: >-
  Tool ran but its result exceeds the result_not_for_model character limit, so
  no result was returned
ccVersion: 2.1.301
variables:
  - TOOL_RESULT_MCP_CALL_RESULT_NOT_FOR_MODEL_OVER_LIMIT_VAR_0
-->
The tool ran, but its result is over the ${TOOL_RESULT_MCP_CALL_RESULT_NOT_FOR_MODEL_OVER_LIMIT_VAR_0}-character limit of an mcp_call sent with result_not_for_model, so this mcp_call got no result. Check whether the call took effect before retrying mcp_call, and ask the tool for a smaller result if you retry.
