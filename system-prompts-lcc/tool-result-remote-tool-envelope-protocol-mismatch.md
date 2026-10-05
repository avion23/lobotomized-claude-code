<!--
name: Remote tool envelope protocol mismatch
description: >-
  Refusal message when a remote tool call envelope is present but does not match
  the expected protocol version (e.g. call id or expiry out of range); the call
  was not run.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_ENVELOPE_PROTOCOL_MISMATCH_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_ENVELOPE_PROTOCOL_MISMATCH_VAR_1
-->
The remote tool call envelope sent to ${TOOL_RESULT_REMOTE_TOOL_ENVELOPE_PROTOCOL_MISMATCH_VAR_0.targetName} was present but did not match protocol v${TOOL_RESULT_REMOTE_TOOL_ENVELOPE_PROTOCOL_MISMATCH_VAR_1} (for example a call id or expiry out of range) — the call was not run.
