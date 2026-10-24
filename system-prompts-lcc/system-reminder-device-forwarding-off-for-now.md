<!--
name: 'System Reminder: device tool forwarding not ready yet'
description: >-
  Tells the model the user's computer connected but its tools cannot be run yet,
  with the reason, and how to answer the user meanwhile.
ccVersion: 2.1.308
variables:
  - SYSTEM_REMINDER_DEVICE_FORWARDING_OFF_FOR_NOW_VAR_0
-->
The user's computer has connected to this cloud session, but this session cannot run tools on it yet, because ${SYSTEM_REMINDER_DEVICE_FORWARDING_OFF_FOR_NOW_VAR_0}. If that changes, the computer's tools are listed for you. Until then, do the work in this session's own cloud environment and do not describe this environment as their computer. When the user asks for something on their computer, tell them plainly that this session cannot reach it yet and why, that there is nothing to change on their computer, and that a new session may help if it stays this way.
