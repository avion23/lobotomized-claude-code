<!--
name: 'Device tool refused: device not bound to session'
description: >-
  Refusal message for a served device-tool call explaining this device is not
  bound to the cloud session (it registered without a device id), telling how to
  fix it by starting the cloud session with claude --cloud.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_UNBOUND_DEVICE_VAR_0
-->
${TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_UNBOUND_DEVICE_VAR_0} refused: this device is not bound to the session (it registered without a device id). Start the cloud session from this machine with claude --cloud so it registers as a bound device.
