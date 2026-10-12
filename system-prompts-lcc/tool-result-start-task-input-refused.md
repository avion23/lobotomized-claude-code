<!--
name: 'Tool Result: Start task input refused'
description: >-
  start_task refusal envelope: "Cannot call start_task with these arguments:"
  followed by the listed problems, any file problem, the arguments the tool
  takes and what was not done.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_START_TASK_INPUT_REFUSED_VAR_0
  - TOOL_RESULT_START_TASK_INPUT_REFUSED_VAR_1
  - TOOL_RESULT_START_TASK_INPUT_REFUSED_VAR_2
-->
Cannot call start_task with these arguments: ${TOOL_RESULT_START_TASK_INPUT_REFUSED_VAR_0.listed}.${TOOL_RESULT_START_TASK_INPUT_REFUSED_VAR_1}${TOOL_RESULT_START_TASK_INPUT_REFUSED_VAR_0.takes} ${TOOL_RESULT_START_TASK_INPUT_REFUSED_VAR_2}
