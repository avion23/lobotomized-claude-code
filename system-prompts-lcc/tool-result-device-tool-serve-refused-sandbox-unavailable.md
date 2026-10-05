<!--
name: 'Device tool refused: sandbox not enabled'
description: >-
  Refusal message for a served device-tool call explaining sandboxing is not
  enabled on this device and device tools are only served from a sandboxed
  machine, instructing how to enable it and check with /sandbox.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_SANDBOX_UNAVAILABLE_VAR_0
-->
${TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_SANDBOX_UNAVAILABLE_VAR_0} refused: sandboxing is not enabled on this device, and device tools are only served from a machine whose Claude Code sandbox is on. Ask the user to set "sandbox": {"enabled": true} in Claude Code settings on the device (check with /sandbox); do not retry until they have.
