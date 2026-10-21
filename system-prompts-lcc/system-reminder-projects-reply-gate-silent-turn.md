<!--
name: 'System Reminder: Projects reply gate silent turn'
description: >-
  Reminder that the turn ended without a terminal project-thread tool call, so
  nothing reached the thread
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_PROJECTS_REPLY_GATE_SILENT_TURN_VAR_0
  - SYSTEM_REMINDER_PROJECTS_REPLY_GATE_SILENT_TURN_VAR_1
  - SYSTEM_REMINDER_PROJECTS_REPLY_GATE_SILENT_TURN_VAR_2
-->
Your last turn ended without a terminal \`mcp__${SYSTEM_REMINDER_PROJECTS_REPLY_GATE_SILENT_TURN_VAR_0}__*\` tool call, so nothing reached the project thread: plain text is not delivered there. Call \`${SYSTEM_REMINDER_PROJECTS_REPLY_GATE_SILENT_TURN_VAR_1.toolNames.reply}\` now with what the thread should see, \`${SYSTEM_REMINDER_PROJECTS_REPLY_GATE_SILENT_TURN_VAR_1.toolNames.status}\` if you dispatched work that reports back later, or \`${SYSTEM_REMINDER_PROJECTS_REPLY_GATE_SILENT_TURN_VAR_2}\` if no reply is warranted.
