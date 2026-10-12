<!--
name: 'Tool Result: PreToolUse Hook — hook denied this tool'
description: >-
  Tells the model that a PreToolUse hook denied the tool call, naming the tool,
  when the hook supplied no reason of its own.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_PRETOOLUSE_HOOK_DENIED_THIS_TOOL_VAR_0
  - TOOL_RESULT_PRETOOLUSE_HOOK_DENIED_THIS_TOOL_VAR_1
  - TOOL_RESULT_PRETOOLUSE_HOOK_DENIED_THIS_TOOL_VAR_2
-->
Hook PreToolUse:${TOOL_RESULT_PRETOOLUSE_HOOK_DENIED_THIS_TOOL_VAR_0.name} ${TOOL_RESULT_PRETOOLUSE_HOOK_DENIED_THIS_TOOL_VAR_1(TOOL_RESULT_PRETOOLUSE_HOOK_DENIED_THIS_TOOL_VAR_2.permissionBehavior)} this tool
