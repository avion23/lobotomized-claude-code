<!--
name: Artifact auto-reply kill-all disclosure
description: >-
  Task notification body that the user stopped artifact watches or auto-replies
  and wakes stay off
ccVersion: 2.1.310
variables:
  - DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_0
  - DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_1
  - DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_2
  - DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_3
  - DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_4
-->

${DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_0(DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_1.map(DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_2).concat([DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_3?DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_4>0?"Comments sent to Claude no longer wake this session. Wakes stay off until the user restarts Claude Code and publishes again.":"No watch was active to stop. Wakes stay off until the user restarts Claude Code and publishes again.":DATA_TASK_NOTIFICATION_ARTIFACT_AUTO_REPLY_KILL_ALL_DISCLOSURE_VAR_4>0?"Auto-replies are disarmed for the rest of this session (a new session re-arms on publish; a watch this session carried is ended or stays disarmed for its continuations).":"No subscription was active to stop (a new session re-arms on publish; a watch this session carried stays disarmed for its continuations)."]).join(`

`))}
