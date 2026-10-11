<!--
name: 'Tool Result: Start task input — takes arguments'
description: >-
  Sentence appended to a start_task input refusal listing every argument the
  tool takes, required ones marked.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_START_TASK_INPUT_TAKES_ARGUMENTS_VAR_0
  - TOOL_RESULT_START_TASK_INPUT_TAKES_ARGUMENTS_VAR_1
-->
 ${TOOL_RESULT_START_TASK_INPUT_TAKES_ARGUMENTS_VAR_0.tool} takes ${TOOL_RESULT_START_TASK_INPUT_TAKES_ARGUMENTS_VAR_1.join(", ")}.
