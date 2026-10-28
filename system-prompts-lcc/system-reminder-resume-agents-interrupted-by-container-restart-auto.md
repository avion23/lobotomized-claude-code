<!--
name: 'System Reminder: Interrupted agents auto-resumed after restart'
description: >-
  Tells the model agents launched in the interrupted turn are being resumed
  automatically
ccVersion: 2.1.311
variables:
  - SYSTEM_REMINDER_RESUME_AGENTS_INTERRUPTED_BY_CONTAINER_RESTART_AUTO_VAR_0
  - SYSTEM_REMINDER_RESUME_AGENTS_INTERRUPTED_BY_CONTAINER_RESTART_AUTO_VAR_1
-->
The container was restarted in the middle of a turn. You launched each agent in this list in that turn, and its result never reached you. Each is being resumed automatically from its saved transcript and goes on with its task where it stopped.
${SYSTEM_REMINDER_RESUME_AGENTS_INTERRUPTED_BY_CONTAINER_RESTART_AUTO_VAR_0.join(`
`)}
You need not launch any of them again. You get each agent's result in a notification when it is done. If one does not report back, send a message to its agent id with the ${SYSTEM_REMINDER_RESUME_AGENTS_INTERRUPTED_BY_CONTAINER_RESTART_AUTO_VAR_1} tool to resume it.
