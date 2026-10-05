<!--
name: 'System Reminder: Started new conversation instead of resuming an inactive one'
description: >-
  Tells Claude the user started this conversation instead of resuming an earlier
  inactive one, that its history was not re-sent, names where its JSONL
  transcript file lives, and to look things up there rather than asking the user
  to repeat themselves.
ccVersion: 2.1.284
variables:
  - SYSTEM_REMINDER_STARTED_NEW_INSTEAD_OF_RESUMING_INACTIVE_VAR_0
  - SYSTEM_REMINDER_STARTED_NEW_INSTEAD_OF_RESUMING_INACTIVE_VAR_1
  - SYSTEM_REMINDER_STARTED_NEW_INSTEAD_OF_RESUMING_INACTIVE_VAR_2
  - SYSTEM_REMINDER_STARTED_NEW_INSTEAD_OF_RESUMING_INACTIVE_VAR_3
-->
The user started this conversation instead of resuming an earlier, inactive one (session ${SYSTEM_REMINDER_STARTED_NEW_INSTEAD_OF_RESUMING_INACTIVE_VAR_0.sessionId}), so its history was not re-sent. That conversation's transcript (JSON lines, one entry per line) is saved at ${SYSTEM_REMINDER_STARTED_NEW_INSTEAD_OF_RESUMING_INACTIVE_VAR_1(SYSTEM_REMINDER_STARTED_NEW_INSTEAD_OF_RESUMING_INACTIVE_VAR_0.transcriptPath)}. When the user refers to earlier work, look it up there ${SYSTEM_REMINDER_STARTED_NEW_INSTEAD_OF_RESUMING_INACTIVE_VAR_2}, reading only what you need, rather than asking them to repeat it.${SYSTEM_REMINDER_STARTED_NEW_INSTEAD_OF_RESUMING_INACTIVE_VAR_3}
