<!--
name: 'Tool Description: Save task files arguments'
description: >-
  Shared sentence on passing task_id and each file's id, name and size from
  get_task
ccVersion: 2.1.311
variables:
  - TOOL_DESCRIPTION_SAVE_TASK_FILES_PASS_TASK_FILES_VAR_0
-->
Pass the task's task_id and, for up to ${TOOL_DESCRIPTION_SAVE_TASK_FILES_PASS_TASK_FILES_VAR_0} of its files, the file's id, the name it is saved as and its size in bytes, each exactly as a get_task answer for that task gave them earlier in this session: the saved-as name is the name the task gave the file, made safe as a file name, and the answer's note spells it out where the two differ or the name is long.
