<!--
name: 'Tool Result: Auto mode unavailable, continue without'
description: >-
  Deny message when auto mode's safety check does not run for this session:
  other actions needing it will be denied too; finish what is possible and tell
  the user
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AUTO_MODE_UNAVAILABLE_CONTINUE_WITHOUT_VAR_0
-->
Auto mode is unavailable: its safety check does not run for this session, so ${TOOL_RESULT_AUTO_MODE_UNAVAILABLE_CONTINUE_WITHOUT_VAR_0.name} was not run. Other actions that need the check will be denied too, and retrying won't help. Finish what you can without them, then tell the user what is blocked and that they can switch to another permission mode.
