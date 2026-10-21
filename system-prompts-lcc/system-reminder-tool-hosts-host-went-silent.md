<!--
name: 'System Reminder: Tool hosts host went silent'
description: >-
  Tool hosts listing line that an attached machine is not reachable after it
  stopped answering checks without saying why
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_HOST_WENT_SILENT_VAR_0
  - SYSTEM_REMINDER_TOOL_HOSTS_HOST_WENT_SILENT_VAR_1
-->
- ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_WENT_SILENT_VAR_0}: not reachable: ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_WENT_SILENT_VAR_1===void 0?"":`last heard from at ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_WENT_SILENT_VAR_1}, then `}it stopped answering this session's checks without saying why, which most often means Claude on ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_WENT_SILENT_VAR_0} is no longer running (the app was closed, say) or lost its connection, or the computer went to sleep or offline; what brings it back is Claude open on ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_WENT_SILENT_VAR_0} again with the computer awake and online.
