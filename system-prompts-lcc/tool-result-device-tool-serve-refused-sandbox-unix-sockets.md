<!--
name: 'Device tool refused: sandbox allows Unix sockets'
description: >-
  Refusal message for a served device-tool call explaining the device's sandbox
  allows connections to Unix sockets, through which a command could reach
  services outside the sandbox, so it serves no device tools.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_SANDBOX_UNIX_SOCKETS_VAR_0
-->
${TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_SANDBOX_UNIX_SOCKETS_VAR_0} refused: the sandbox on this device allows connections to Unix sockets (sandbox.network.allowAllUnixSockets or allowUnixSockets), through which a command could reach services running outside the sandbox, so this device serves no device tools. Tell the user; do not retry in a loop.
