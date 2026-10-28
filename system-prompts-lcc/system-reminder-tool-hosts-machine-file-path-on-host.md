<!--
name: 'System Reminder: Tool hosts machine file paths on host'
description: >-
  Explains how file tools with the machine argument act on the user's current
  files there and must use absolute paths on that machine
ccVersion: 2.1.310
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_0
  - SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_1
  - SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_2
  - SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_3
  - SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_4
  - SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_5
-->
${SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_0(SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_1)} ${SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_2} ${SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_3} on the user's current files there, under that machine's own permission rules — give paths (file_path, or a search's path) as absolute paths on that machine; without "${SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_4}" they act on this session's snapshot. Searches made without "${SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_4}" only see this session's snapshot: to search the user's current files ${SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_FILE_PATH_ON_HOST_VAR_5}
