<!--
name: 'System Reminder: Tool hosts separate copy lives there'
description: >-
  Explains that the user's separate copy of the project is on the named machine,
  may differ from this checkout, and is not synced
ccVersion: 2.1.310
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_SEPARATE_COPY_LIVES_THERE_VAR_0
-->
The user's own separate copy of the project is on ${SYSTEM_REMINDER_TOOL_HOSTS_MACHINE_SEPARATE_COPY_LIVES_THERE_VAR_0} — it may be at a different commit than this session's checkout, or hold uncommitted work that is not here — along with their other files, applications, local toolchains and running processes. A call run there acts on that copy only, and nothing is synced between it and this session's checkout in either direction; its own Claude Code decides what may run there and may ask the user first.
