<!--
name: 'System Reminder: Device MCP serving not now (detailed)'
description: >-
  Notice that this machine's MCP servers are not offered because the user chose
  Not now, and claude --cloud asks again once one is added
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_DEVICE_MCP_SERVING_NOT_NOW_DETAILED_VAR_0
-->
This machine has MCP servers a cloud session could use through it; none are offered: you chose Not now for these servers, so claude --cloud asks again once you add one (${SYSTEM_REMINDER_DEVICE_MCP_SERVING_NOT_NOW_DETAILED_VAR_0()}).
