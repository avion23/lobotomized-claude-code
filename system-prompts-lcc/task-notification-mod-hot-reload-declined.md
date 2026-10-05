<!--
name: 'Task Notification: Mod hot-reloading declined'
description: >-
  Tells Claude the person declined mod hot-reloading, so what this run wrote
  under the mods directory is written but NOT loaded, not to say the change is
  running, and that it loads next time the session starts.
ccVersion: 2.1.284
variables:
  - TASK_NOTIFICATION_MOD_HOT_RELOAD_DECLINED_VAR_0
-->
The person declined mod hot-reloading: what this run wrote under ${TASK_NOTIFICATION_MOD_HOT_RELOAD_DECLINED_VAR_0} is written but NOT loaded (a mod that loaded when the session started keeps running as it loaded). Do not say the change is running. It loads the next time this session starts (/reload-plugins reloads only a mod that loaded at the start); the person can ask again.
