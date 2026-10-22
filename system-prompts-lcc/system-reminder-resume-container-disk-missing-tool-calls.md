<!--
name: 'System Reminder: resumed container disk missing tool calls'
description: >-
  Warns on resume that the container's disk lacks recent tool calls, so
  files/packages may be missing; check and tell the user.
ccVersion: 2.1.308
variables:
  - SYSTEM_REMINDER_RESUME_CONTAINER_DISK_MISSING_TOOL_CALLS_VAR_0
-->
When this session resumed, the copy of this conversation on the container's disk lacked at least ${SYSTEM_REMINDER_RESUME_CONTAINER_DISK_MISSING_TOOL_CALLS_VAR_0} of your recent tool calls, so the disk may be older than the conversation. Files that those calls created or changed may be missing or out of date, and installed packages may be gone. Check the files that you need before you rely on them, and tell the user if work was lost.
