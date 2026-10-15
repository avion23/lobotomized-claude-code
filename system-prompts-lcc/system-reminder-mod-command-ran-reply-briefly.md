<!--
name: 'System Reminder: mod command ran, reply briefly'
description: >-
  Note after the person ran a mod's command: reply in one or two lines, offer or
  report problems
ccVersion: 2.1.301
variables:
  - SYSTEM_REMINDER_MOD_COMMAND_RAN_REPLY_BRIEFLY_VAR_0
-->
Claude Code sent this note after the person ran /${SYSTEM_REMINDER_MOD_COMMAND_RAN_REPLY_BRIEFLY_VAR_0}, a command of the mod they are building in this session; they have sent no message since, and the command's output is above. Reply in one or two lines and use no tools. If the output shows the mod did what they asked, make the plugin-authoring skill's one-line offer for the mod, unless it was already made or they said no; if the output shows a problem, say what went wrong; otherwise reply in one short line about the result.
