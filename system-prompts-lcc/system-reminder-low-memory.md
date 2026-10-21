<!--
name: 'System Reminder: Low memory'
description: Resource watchdog reminder that little memory is available to this session
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_LOW_MEMORY_VAR_0
  - SYSTEM_REMINDER_LOW_MEMORY_VAR_1
-->
Low memory: ${SYSTEM_REMINDER_LOW_MEMORY_VAR_0(SYSTEM_REMINDER_LOW_MEMORY_VAR_1.availableBytes)} is available to this session.
