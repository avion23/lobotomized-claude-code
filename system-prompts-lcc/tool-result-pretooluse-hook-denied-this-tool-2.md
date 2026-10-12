<!--
name: 'Tool Result: PreToolUse Hook — hook denied this tool'
description: >-
  Tells the model that a PreToolUse hook denied the tool call, naming the tool,
  when the hook supplied no reason of its own.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_PRETOOLUSE_HOOK_DENIED_THIS_TOOL_2_VAR_0
  - TOOL_RESULT_PRETOOLUSE_HOOK_DENIED_THIS_TOOL_2_VAR_1
-->
Hook PreToolUse:${TOOL_RESULT_PRETOOLUSE_HOOK_DENIED_THIS_TOOL_2_VAR_0.tool} ${TOOL_RESULT_PRETOOLUSE_HOOK_DENIED_THIS_TOOL_2_VAR_1("deny")} this tool
