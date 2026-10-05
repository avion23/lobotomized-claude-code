<!--
name: 'Device MCP tools not offered, with reasons'
description: >-
  Notice listing which tools were not offered to the cloud session and why, up
  to six with a '+N more' tail.
ccVersion: 2.1.284
variables:
  - SYSTEM_REMINDER_DEVICE_MCP_SERVING_NOT_OFFERED_LIST_VAR_0
  - SYSTEM_REMINDER_DEVICE_MCP_SERVING_NOT_OFFERED_LIST_VAR_1
-->
Not offered to the cloud session: ${SYSTEM_REMINDER_DEVICE_MCP_SERVING_NOT_OFFERED_LIST_VAR_0}${SYSTEM_REMINDER_DEVICE_MCP_SERVING_NOT_OFFERED_LIST_VAR_1.length>6?`, and ${SYSTEM_REMINDER_DEVICE_MCP_SERVING_NOT_OFFERED_LIST_VAR_1.length-6} more`:""}.
