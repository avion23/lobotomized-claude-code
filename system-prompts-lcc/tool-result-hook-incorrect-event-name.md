<!--
name: 'Tool Result: Hook Incorrect Event Name'
description: >-
  Error when a hook's JSON output names a different hookEventName than the event
  it ran for.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_HOOK_INCORRECT_EVENT_NAME_VAR_0
  - TOOL_RESULT_HOOK_INCORRECT_EVENT_NAME_VAR_1
  - TOOL_RESULT_HOOK_INCORRECT_EVENT_NAME_VAR_2
-->
Hook returned incorrect event name: expected '${TOOL_RESULT_HOOK_INCORRECT_EVENT_NAME_VAR_0}' but got '${TOOL_RESULT_HOOK_INCORRECT_EVENT_NAME_VAR_1.hookSpecificOutput.hookEventName}'. Full stdout: ${TOOL_RESULT_HOOK_INCORRECT_EVENT_NAME_VAR_2(TOOL_RESULT_HOOK_INCORRECT_EVENT_NAME_VAR_1,null,2)}
