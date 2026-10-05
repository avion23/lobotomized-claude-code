<!--
name: Call larger than target accepts
description: >-
  Refusal message when a call's request body exceeds the target's
  max_request_bytes limit; the call was not run.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_CALL_TOO_LARGE_FOR_TARGET_VAR_0
-->
The call is larger than ${TOOL_RESULT_REMOTE_TOOL_CALL_TOO_LARGE_FOR_TARGET_VAR_0.targetName} accepts (${TOOL_RESULT_REMOTE_TOOL_CALL_TOO_LARGE_FOR_TARGET_VAR_0.policy.limits.max_request_bytes} bytes) — it was not run.
