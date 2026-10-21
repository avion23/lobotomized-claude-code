<!--
name: 'System Reminder: Tool hosts host asleep'
description: >-
  Tool hosts listing line that an attached machine is not reachable since it
  said its computer was going to sleep
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_HOST_ASLEEP_VAR_0
  - SYSTEM_REMINDER_TOOL_HOSTS_HOST_ASLEEP_VAR_1
-->
- ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_ASLEEP_VAR_0}: not reachable since ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_ASLEEP_VAR_1===void 0?"":`${SYSTEM_REMINDER_TOOL_HOSTS_HOST_ASLEEP_VAR_1}, when `}it said its computer was going to sleep; what brings it back is the computer waking, nothing more.
