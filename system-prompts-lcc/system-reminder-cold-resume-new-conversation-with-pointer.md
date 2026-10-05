<!--
name: 'System Reminder: Cold resume new-conversation notice (with pointer)'
description: >-
  Notice inserted into the transcript when a cold-resume quota warning starts a
  new conversation, telling Claude it can look up a quoted excerpt of the
  previous conversation if the user refers to it
ccVersion: 2.1.284
variables:
  - SYSTEM_REMINDER_COLD_RESUME_NEW_CONVERSATION_WITH_POINTER_VAR_0
  - SYSTEM_REMINDER_COLD_RESUME_NEW_CONVERSATION_WITH_POINTER_VAR_1
-->
New conversation. Claude can look up "${SYSTEM_REMINDER_COLD_RESUME_NEW_CONVERSATION_WITH_POINTER_VAR_0(SYSTEM_REMINDER_COLD_RESUME_NEW_CONVERSATION_WITH_POINTER_VAR_1,60)}" if you refer to it.
