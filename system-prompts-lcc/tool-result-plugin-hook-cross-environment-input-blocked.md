<!--
name: Hook cross-environment input blocked
description: >-
  Tells the model a hook changed input for a call in another environment, so the
  call was not made.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_PLUGIN_HOOK_CROSS_ENVIRONMENT_INPUT_BLOCKED_VAR_0
  - TOOL_RESULT_PLUGIN_HOOK_CROSS_ENVIRONMENT_INPUT_BLOCKED_VAR_1
-->
${TOOL_RESULT_PLUGIN_HOOK_CROSS_ENVIRONMENT_INPUT_BLOCKED_VAR_0} changed this tool call's input. That is allowed only for calls that run in the same environment as the hook, and this one does not, so the call was not made. Retrying will not help while the hook keeps changing the input. Go on without this call, and tell the user that a hook in ${TOOL_RESULT_PLUGIN_HOOK_CROSS_ENVIRONMENT_INPUT_BLOCKED_VAR_1} changes this tool's input, which is not supported here.
