<!--
name: Artifact comment read thread
description: >-
  Notification detail telling Claude to read a comment thread and make an
  appropriate change in the artifact source and publish again
ccVersion: 2.1.310
variables:
  - DATA_TASK_NOTIFICATION_ARTIFACT_COMMENT_READ_THREAD_VAR_0
  - DATA_TASK_NOTIFICATION_ARTIFACT_COMMENT_READ_THREAD_VAR_1
  - DATA_TASK_NOTIFICATION_ARTIFACT_COMMENT_READ_THREAD_VAR_2
  - DATA_TASK_NOTIFICATION_ARTIFACT_COMMENT_READ_THREAD_VAR_3
-->
${DATA_TASK_NOTIFICATION_ARTIFACT_COMMENT_READ_THREAD_VAR_0}. Read it with ${DATA_TASK_NOTIFICATION_ARTIFACT_COMMENT_READ_THREAD_VAR_1}, passing slug "${DATA_TASK_NOTIFICATION_ARTIFACT_COMMENT_READ_THREAD_VAR_2}" and thread "${DATA_TASK_NOTIFICATION_ARTIFACT_COMMENT_READ_THREAD_VAR_3}". If it asks for a change to the artifact and the change is appropriate, make it first, in the artifact's source (the local file you published it from, if any), and publish again.
