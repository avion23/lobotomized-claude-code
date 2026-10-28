<!--
name: 'System Reminder: Tool hosts separate copy machine-arg file tools'
description: >-
  Explains that file tools with the machine argument act on the user's copy
  there, take absolute paths, and that the two copies may differ
ccVersion: 2.1.310
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_0
  - SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_1
  - SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_2
  - SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_3
  - SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_4
  - SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_5
-->
${SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_0(SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_1)} ${SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_2} ${SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_3} on the user's copy there, under that machine's own permission rules — give paths (file_path, or a search's path) as absolute paths on that machine${SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_4}; without "${SYSTEM_REMINDER_TOOL_HOSTS_SEPARATE_COPY_MACHINE_ARG_FILE_TOOLS_VAR_5}" they act on this session's checkout. The same relative path names two different files, one in each copy, and they may differ: an edit to one does not change the other
