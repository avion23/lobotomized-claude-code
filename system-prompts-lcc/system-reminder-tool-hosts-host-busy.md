<!--
name: 'System Reminder: Tool hosts host busy'
description: >-
  Tool hosts listing line that an attached machine is not reachable because it
  said it was busy running a command, so the connection is down
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_HOST_BUSY_VAR_0
  - SYSTEM_REMINDER_TOOL_HOSTS_HOST_BUSY_VAR_1
-->
- ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_BUSY_VAR_0}: not reachable: ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_BUSY_VAR_1===void 0?"":`it last replied at ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_BUSY_VAR_1}, and `}its only word since was that it was busy running a command and could not hear this session, so Claude there and the computer are most likely fine and its connection to this session is what is down; what brings it back is that computer's network, and quitting Claude there would stop the command it is running.
