<!--
name: 'System Reminder: Low disk space'
description: >-
  Resource watchdog reminder that only a little disk space is free on the
  filesystem holding the working directory
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_LOW_DISK_SPACE_VAR_0
  - SYSTEM_REMINDER_LOW_DISK_SPACE_VAR_1
-->
Low disk space: ${SYSTEM_REMINDER_LOW_DISK_SPACE_VAR_0(SYSTEM_REMINDER_LOW_DISK_SPACE_VAR_1)} is free on the filesystem holding the working directory.
