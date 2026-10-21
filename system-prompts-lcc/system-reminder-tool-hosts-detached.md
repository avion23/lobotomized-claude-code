<!--
name: 'System Reminder: Tool hosts detached'
description: >-
  Notice that no machine is attached any more, to omit the machine parameter and
  say so if the task needs that machine
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_DETACHED_VAR_0
  - SYSTEM_REMINDER_TOOL_HOSTS_DETACHED_VAR_1
-->
${SYSTEM_REMINDER_TOOL_HOSTS_DETACHED_VAR_0}; omit "${SYSTEM_REMINDER_TOOL_HOSTS_DETACHED_VAR_1}" and run commands here. If the task needs that machine's files, tools or logins, say so instead of doing it here.
