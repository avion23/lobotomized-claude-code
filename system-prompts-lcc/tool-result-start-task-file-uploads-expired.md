<!--
name: Start task file uploads expired
description: >-
  Requires fresh uploads when a task approval uses attachments that are
  expiring.
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_START_TASK_FILE_UPLOADS_EXPIRED_VAR_2
  - TOOL_RESULT_START_TASK_FILE_UPLOADS_EXPIRED_VAR_0
-->
The files for this task were uploaded about an hour before this approval and have expired or are about to. Call ${TOOL_RESULT_START_TASK_FILE_UPLOADS_EXPIRED_VAR_2} again to upload them afresh. ${TOOL_RESULT_START_TASK_FILE_UPLOADS_EXPIRED_VAR_0.words.nothingDone}
