<!--
name: 'Device tool refused: sandbox not fully confining'
description: >-
  Refusal message for a served device-tool call explaining the device's sandbox
  is not fully confining (filesystem and network), with the settings fix and a
  note not to run subprocess-env-scrub mode.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_SANDBOX_UNCONFINED_VAR_0
-->
${TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_SANDBOX_UNCONFINED_VAR_0} refused: the sandbox on this device is not fully confining (filesystem and network). Ask the user to set "sandbox": {"enabled": true, "filesystem": {"disabled": false}} in Claude Code settings on the device and not to run it in subprocess-env-scrub mode; do not retry until they have.
