<!--
name: 'System Reminder: Container restart, agents resuming'
description: >-
  Notice that the container restarted mid-turn and unanswered Agent calls are
  being resumed from their transcripts; wait for their notifications
ccVersion: 2.1.312
variables:
  - SYSTEM_REMINDER_CONTAINER_RESTART_AGENTS_RESUMING_VAR_0
  - SYSTEM_REMINDER_CONTAINER_RESTART_AGENTS_RESUMING_VAR_1
-->
The container was restarted in the middle of a turn. Every Agent call that turn left unanswered is being resumed automatically from its saved transcript, as these agents: ${SYSTEM_REMINDER_CONTAINER_RESTART_AGENTS_RESUMING_VAR_0.join(", ")}. Wait for their notifications, which name each agent's task and give its result, before you do that work again. If one does not report back, send a message to its agent id with the ${SYSTEM_REMINDER_CONTAINER_RESTART_AGENTS_RESUMING_VAR_1} tool to resume it.
