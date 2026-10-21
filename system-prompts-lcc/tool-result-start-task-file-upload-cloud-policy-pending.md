<!--
name: 'Tool result: start_task cloud environment policy not loaded'
description: >-
  Error returned when the cloud environment has not yet loaded the
  organization's policy, so file uploads cannot be judged.
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_START_TASK_FILE_UPLOAD_CLOUD_POLICY_PENDING_VAR_0
  - TOOL_RESULT_START_TASK_FILE_UPLOAD_CLOUD_POLICY_PENDING_VAR_1
-->
This session's cloud environment has not yet loaded its organization's policy, so it cannot tell whether files may be uploaded. ${TOOL_RESULT_START_TASK_FILE_UPLOAD_CLOUD_POLICY_PENDING_VAR_0} Try again in a moment, or ${TOOL_RESULT_START_TASK_FILE_UPLOAD_CLOUD_POLICY_PENDING_VAR_1.offerWithoutFiles}.
