<!--
name: Device hook blocking stderr
description: Blocking hook answer carrying the hook label and its stderr output.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_DEVICE_HOOK_BLOCKING_STDERR_VAR_0
  - TOOL_RESULT_DEVICE_HOOK_BLOCKING_STDERR_VAR_1
-->
[${TOOL_RESULT_DEVICE_HOOK_BLOCKING_STDERR_VAR_0}]: ${TOOL_RESULT_DEVICE_HOOK_BLOCKING_STDERR_VAR_1.stderr||"No stderr output"}
