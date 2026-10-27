<!--
name: 'Tool Result: Task files save instructions'
description: >-
  Tells Claude how to call the save tool with task_id and each file's file_id,
  bytes and save_as
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_MANAGED_AGENTS_TASK_FILES_SAVE_INSTRUCTIONS_VAR_0
-->
To save some, call ${TOOL_RESULT_MANAGED_AGENTS_TASK_FILES_SAVE_INSTRUCTIONS_VAR_0} with this task's task_id and, for each file, its id as file_id, its size as bytes, and as save_as the save_as on its line if one is given, else its name; names here are JSON strings, so give save_as as the same string.
