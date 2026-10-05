<!--
name: 'Task Notification: Mod hot-reloading question unanswered'
description: >-
  Tells Claude the mod hot-reloading question hasn't been answered yet and will
  be asked again once the turn ends, that what this run wrote isn't loaded yet,
  and not to say it was declined or suggest --plugin-dir/a restart.
ccVersion: 2.1.284
variables:
  - TASK_NOTIFICATION_MOD_HOT_RELOAD_UNANSWERED_VAR_0
-->
The person has not answered the mod hot-reloading question yet; it is asked again once a turn ends. What this run wrote under ${TASK_NOTIFICATION_MOD_HOT_RELOAD_UNANSWERED_VAR_0} is written but NOT loaded yet. Do not say it was declined, and do not suggest --plugin-dir or a restart.
