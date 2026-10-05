<!--
name: Passthrough server tools changed
description: >-
  Tool-result denial message when the target MCP server changed its tool list
  since approval and the call is withheld pending re-approval.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_DEVICE_MCP_PASSTHROUGH_TOOLS_CHANGED_VAR_0
  - TOOL_RESULT_DEVICE_MCP_PASSTHROUGH_TOOLS_CHANGED_VAR_1
-->
MCP server "${TOOL_RESULT_DEVICE_MCP_PASSTHROUGH_TOOLS_CHANGED_VAR_0(TOOL_RESULT_DEVICE_MCP_PASSTHROUGH_TOOLS_CHANGED_VAR_1)}" changed the tools it lists since you approved offering it; the call did not run (claude --cloud asks at the next start)
