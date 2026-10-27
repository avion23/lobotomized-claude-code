<!--
name: 'Tool Result: Remote tool background task output file is not status'
description: >-
  Tool-result note that a command keeps running as a background task on the
  machine, how to read its output and stop it, and never to use pgrep, pkill or
  kill
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_1
  - TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_2
  - TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_3
-->
(that command keeps running as a background task ON ${TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_0}: its ID and output file exist there, not here, and this session is not notified when it finishes. Its output file there (${TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_1} with ${TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_2}: "${TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_0}") shows what it has printed, not whether it is still running. To stop it, call ${TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_3} with that ID and ${TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_2}: "${TOOL_RESULT_REMOTE_TOOL_BACKGROUND_TASK_OUTPUT_FILE_NOT_STATUS_VAR_0}". Never check on it or stop it with pgrep, pkill or kill: with the sandbox on there, a later command cannot see or reach this process, or a server it started. To test such a server, do it inside the same command, or ask the user to turn the sandbox off for that folder.)
