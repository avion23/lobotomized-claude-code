<!--
name: 'Tool Result: Cron scheduled one-shot'
description: >-
  Confirms a one-shot scheduled task, its schedule and that it auto-deletes
  after firing
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_CRON_SCHEDULED_ONESHOT_VAR_0
  - TOOL_RESULT_CRON_SCHEDULED_ONESHOT_VAR_1
  - TOOL_RESULT_CRON_SCHEDULED_ONESHOT_VAR_2
-->
Scheduled one-shot task ${TOOL_RESULT_CRON_SCHEDULED_ONESHOT_VAR_0.id} (${TOOL_RESULT_CRON_SCHEDULED_ONESHOT_VAR_0.humanSchedule}).${TOOL_RESULT_CRON_SCHEDULED_ONESHOT_VAR_1} ${TOOL_RESULT_CRON_SCHEDULED_ONESHOT_VAR_2}. It will fire once then auto-delete.
