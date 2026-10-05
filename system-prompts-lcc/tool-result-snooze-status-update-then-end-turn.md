<!--
name: 'Tool Result: Snooze status update then end turn'
description: >-
  Wakeup-scheduled result telling the agent to send any owed status update this
  tick, then end the turn until the harness re-invokes it.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_SNOOZE_STATUS_UPDATE_THEN_END_TURN_VAR_0
-->
If you owe the user a status update this tick, ${TOOL_RESULT_SNOOZE_STATUS_UPDATE_THEN_END_TURN_VAR_0}; then end the turn — the harness re-invokes you when the wakeup fires or a task-notification arrives.
