<!--
name: Request computer stub result
description: This call did not connect a computer; use remote-device tools if present.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_REQUEST_COMPUTER_STUB_VAR_0
  - TOOL_RESULT_REQUEST_COMPUTER_STUB_VAR_1
-->
This call did not connect a computer, and no tool here can. Tools whose names start with mcp__${TOOL_RESULT_REQUEST_COMPUTER_STUB_VAR_0}__, if you have any, run on the user's computer; use whichever of them fits the task, loading it with ${TOOL_RESULT_REQUEST_COMPUTER_STUB_VAR_1} first, and waiting for that result, if it was only announced as available there and has not been loaded since. Otherwise carry on with the tools you have here, and if the task needs the user's computer, tell the user so.
