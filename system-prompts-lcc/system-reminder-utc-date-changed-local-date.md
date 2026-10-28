<!--
name: 'System Reminder: UTC date changed (local date may differ)'
description: >-
  Date-change reminder when the date is assumed UTC, telling Claude that a
  non-UTC date in a user's system-reminder is the user's local date
ccVersion: 2.1.312
variables:
  - SYSTEM_REMINDER_UTC_DATE_CHANGED_LOCAL_DATE_VAR_0
-->
The UTC date is now ${SYSTEM_REMINDER_UTC_DATE_CHANGED_LOCAL_DATE_VAR_0.date}. The user's local date can differ. If a system-reminder in a user's message, other than an earlier "Today's date is" line (that was the UTC date), gives a date or time that is not marked UTC, that is the user's local date: treat it as today's date.
