<!--
name: 'System Reminder: Tool host correction — call ended with an error there'
description: >-
  Late correction telling Claude that an attached machine now reports a given-up
  call ended there with an error that was recorded there and not delivered to
  this session
ccVersion: 2.1.310
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_CORRECTION_ENDED_WITH_ERROR_VAR_0
  - SYSTEM_REMINDER_TOOL_HOSTS_CORRECTION_ENDED_WITH_ERROR_VAR_1
  - SYSTEM_REMINDER_TOOL_HOSTS_CORRECTION_ENDED_WITH_ERROR_VAR_2
-->
${SYSTEM_REMINDER_TOOL_HOSTS_CORRECTION_ENDED_WITH_ERROR_VAR_0} That machine now reports it ended there with an error (recorded there, not delivered here): the command ran and failed, or was refused before it started. ${SYSTEM_REMINDER_TOOL_HOSTS_CORRECTION_ENDED_WITH_ERROR_VAR_1(SYSTEM_REMINDER_TOOL_HOSTS_CORRECTION_ENDED_WITH_ERROR_VAR_2)}
