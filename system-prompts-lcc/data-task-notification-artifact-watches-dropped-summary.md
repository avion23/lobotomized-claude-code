<!--
name: 'Task notification: artifact watches dropped summary'
description: >-
  Task-notification summary that the session stopped watching artifacts because
  the account signed out or changed.
ccVersion: 2.1.296
variables:
  - DATA_TASK_NOTIFICATION_ARTIFACT_WATCHES_DROPPED_SUMMARY_VAR_0
  - DATA_TASK_NOTIFICATION_ARTIFACT_WATCHES_DROPPED_SUMMARY_VAR_1
-->
Stopped watching ${DATA_TASK_NOTIFICATION_ARTIFACT_WATCHES_DROPPED_SUMMARY_VAR_0} (${DATA_TASK_NOTIFICATION_ARTIFACT_WATCHES_DROPPED_SUMMARY_VAR_1==="signed_out"?"signed out":"the signed-in account changed"})
