<!--
name: 'Device tool refused: sandbox injects real credentials'
description: >-
  Refusal message for a served device-tool call explaining the device's sandbox
  is configured to inject real credentials into sandboxed network requests, so
  it serves no device tools; tell the user, do not retry in a loop.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_SANDBOX_INJECTS_CREDENTIALS_VAR_0
-->
${TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_SANDBOX_INJECTS_CREDENTIALS_VAR_0} refused: this device's sandbox is configured to inject real credentials into sandboxed network requests (sandbox.credentials entries with mode "mask"), so this device serves no device tools. Tell the user; do not retry in a loop.
