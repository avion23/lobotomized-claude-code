<!--
name: 'Task notification: mod hot-reload enabled but held'
description: >-
  Task-notification text telling Claude the person enabled mod hot-reloading,
  but the mods under a given folder are held for /reload-plugins (since loading
  now would rewrite the prompt cache) and are NOT loaded yet.
ccVersion: 2.1.284
variables:
  - DATA_TASK_NOTIFICATION_MOD_HOT_RELOAD_ENABLED_HELD_VAR_0
-->
The person enabled mod hot-reloading for this session, but the mods under ${DATA_TASK_NOTIFICATION_MOD_HOT_RELOAD_ENABLED_HELD_VAR_0} wait for /reload-plugins (the load would rewrite the prompt cache): they are NOT loaded yet.
