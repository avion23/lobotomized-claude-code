<!--
name: 'Tool Result: device tools refused, sandbox unsupported on this platform'
description: >-
  Refusal text returned when a device tool call is refused because sandboxing is
  enabled in settings but unsupported on this platform/excluded by policy
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_DEVICE_TOOLS_SANDBOX_UNSUPPORTED_PLATFORM_REFUSED_VAR_0
-->
${TOOL_RESULT_DEVICE_TOOLS_SANDBOX_UNSUPPORTED_PLATFORM_REFUSED_VAR_0} refused: sandboxing is enabled in settings on this device but unavailable here (an unsupported platform, or one excluded by an enabledPlatforms policy), so this device serves no device tools. Tell the user; do not retry in a loop.
