<!--
name: Device hook blocking stderr (relabeled)
description: Blocking hook stderr message rebuilt with the hook label in Nn.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_DEVICE_HOOK_BLOCKING_STDERR_RELABELED_VAR_0
  - TOOL_RESULT_DEVICE_HOOK_BLOCKING_STDERR_RELABELED_VAR_1
-->
[${TOOL_RESULT_DEVICE_HOOK_BLOCKING_STDERR_RELABELED_VAR_0.label}]: ${TOOL_RESULT_DEVICE_HOOK_BLOCKING_STDERR_RELABELED_VAR_1.stderr||"No stderr output"}
