<!--
name: 'System Reminder: Tool hosts host shell line'
description: >-
  Host inventory fragment naming the shell that commands run in on an attached
  machine, noting when it is not bash
ccVersion: 2.1.310
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_HOST_SHELL_COMMANDS_RUN_IN_VAR_0
-->
commands run in ${SYSTEM_REMINDER_TOOL_HOSTS_HOST_SHELL_COMMANDS_RUN_IN_VAR_0}${SYSTEM_REMINDER_TOOL_HOSTS_HOST_SHELL_COMMANDS_RUN_IN_VAR_0.includes("bash")?"":", not bash"}
