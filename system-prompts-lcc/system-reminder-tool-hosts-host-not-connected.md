<!--
name: 'System Reminder: Tool hosts host not connected'
description: >-
  Tool hosts listing line that an attached machine is not reachable because its
  Claude is not connected, and what brings it back
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_HOST_NOT_CONNECTED_VAR_0
-->
- ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_NOT_CONNECTED_VAR_0}: not reachable right now: its Claude is not connected to this session (since when is not known), which most often means Claude is not running on ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_NOT_CONNECTED_VAR_0}, Remote Control is off there, or the computer is asleep or offline; what brings it back is Claude open on ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_NOT_CONNECTED_VAR_0} with Remote Control on and the computer awake and online.
