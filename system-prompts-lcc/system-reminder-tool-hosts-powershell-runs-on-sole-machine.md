<!--
name: >-
  System Reminder: Tool hosts — PowerShell runs on the one machine with or
  without the machine argument
description: >-
  PowerShell routing fragment, when only one PowerShell host is attached, saying
  the call runs on that machine whether or not the machine argument is given.
ccVersion: 2.1.296
variables:
  - SYSTEM_REMINDER_TOOL_HOSTS_POWERSHELL_RUNS_ON_SOLE_MACHINE_VAR_0
  - SYSTEM_REMINDER_TOOL_HOSTS_POWERSHELL_RUNS_ON_SOLE_MACHINE_VAR_1
-->
runs on ${SYSTEM_REMINDER_TOOL_HOSTS_POWERSHELL_RUNS_ON_SOLE_MACHINE_VAR_0} with or without "${SYSTEM_REMINDER_TOOL_HOSTS_POWERSHELL_RUNS_ON_SOLE_MACHINE_VAR_1}"
