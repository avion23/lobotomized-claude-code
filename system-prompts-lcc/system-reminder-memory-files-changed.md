<!--
name: 'System Reminder: memory directory — Files changed: …'
description: >-
  Normalized attachment reminder: Files changed: ${.map().join(", ")}. Inserted
  into normalized model context as a meta reminder.
ccVersion: 2.1.296
variables:
  - SYSTEM_REMINDER_MEMORY_FILES_CHANGED_VAR_0
  - SYSTEM_REMINDER_MEMORY_FILES_CHANGED_VAR_1
-->
Files changed: ${SYSTEM_REMINDER_MEMORY_FILES_CHANGED_VAR_0.map(SYSTEM_REMINDER_MEMORY_FILES_CHANGED_VAR_1).join(", ")}
