<!--
name: 'System Reminder: Tool hosts remote background command never notifies'
description: >-
  Warns that a background shell command started on an attached machine never
  notifies this session, and says how to read its output and stop it
ccVersion: 2.1.310
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_REMOTE_BACKGROUND_COMMAND_NEVER_NOTIFIES_VAR_0
  - SYSTEM_REMINDER_TOOL_HOSTS_REMOTE_BACKGROUND_COMMAND_NEVER_NOTIFIES_VAR_1
  - SYSTEM_REMINDER_TOOL_HOSTS_REMOTE_BACKGROUND_COMMAND_NEVER_NOTIFIES_VAR_2
  - SYSTEM_REMINDER_TOOL_HOSTS_REMOTE_BACKGROUND_COMMAND_NEVER_NOTIFIES_VAR_3
-->
- Unlike a background command run here, a ${SYSTEM_REMINDER_TOOL_HOSTS_REMOTE_BACKGROUND_COMMAND_NEVER_NOTIFIES_VAR_0} command started on an attached machine with \`run_in_background\` never notifies this session when it finishes, and nothing re-invokes you for it. When you need to know how it stands, ${SYSTEM_REMINDER_TOOL_HOSTS_REMOTE_BACKGROUND_COMMAND_NEVER_NOTIFIES_VAR_1}: it shows what the command has printed, not whether it is still running. To stop it, call ${SYSTEM_REMINDER_TOOL_HOSTS_REMOTE_BACKGROUND_COMMAND_NEVER_NOTIFIES_VAR_2} with the ID its result gives and "${SYSTEM_REMINDER_TOOL_HOSTS_REMOTE_BACKGROUND_COMMAND_NEVER_NOTIFIES_VAR_3}". Do not end your turn expecting to be woken when it is done.
