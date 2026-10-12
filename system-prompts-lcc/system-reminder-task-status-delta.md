<!--
name: 'Task status reminder: delta'
description: >-
  Normalized attachment reminder: Delta: ${((.deltaSummary))}. Inserted into
  normalized model context as a meta reminder.
ccVersion: 2.1.296
variables:
  - SYSTEM_REMINDER_TASK_STATUS_DELTA_VAR_0
  - SYSTEM_REMINDER_TASK_STATUS_DELTA_VAR_1
  - SYSTEM_REMINDER_TASK_STATUS_DELTA_VAR_2
-->
Delta: ${SYSTEM_REMINDER_TASK_STATUS_DELTA_VAR_0(SYSTEM_REMINDER_TASK_STATUS_DELTA_VAR_1(SYSTEM_REMINDER_TASK_STATUS_DELTA_VAR_2.deltaSummary))}
