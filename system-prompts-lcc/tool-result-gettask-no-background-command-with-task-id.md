<!--
name: 'GetTask: no background command with this task ID (user message)'
description: >-
  Error message returned to the model when GetTask is called with a taskId that
  has no matching background command, explaining where task IDs come from.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_GETTASK_NO_BACKGROUND_COMMAND_WITH_TASK_ID_VAR_0
-->
No background command with task ID ${TOOL_RESULT_GETTASK_NO_BACKGROUND_COMMAND_WITH_TASK_ID_VAR_0}. Task IDs come from the {"resultType":"task", …} result that moved a command to the background, and finished commands are remembered for this session only.
