<!--
name: 'System Reminder: UTC date (local date may differ)'
description: >-
  Current-date reminder when the date is assumed UTC, telling Claude to treat a
  non-UTC date from the user's system-reminder as today's date
ccVersion: 2.1.312
variables:
  - SYSTEM_REMINDER_UTC_DATE_LOCAL_DATE_VAR_0
-->
The UTC date is ${SYSTEM_REMINDER_UTC_DATE_LOCAL_DATE_VAR_0.date}. The user's local date can differ. If a system-reminder in a user's message gives a date or time that is not marked UTC, that is the user's local date: treat it as today's date.
