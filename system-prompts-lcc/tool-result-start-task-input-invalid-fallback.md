<!--
name: 'Tool Result: Start task input — invalid (fallback)'
description: >-
  Fallback start_task input refusal clause for any other schema failure: the
  field (or the arguments) followed by the validator message, or "are not
  valid".
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_START_TASK_INPUT_INVALID_FALLBACK_VAR_0
  - TOOL_RESULT_START_TASK_INPUT_INVALID_FALLBACK_VAR_1
-->
${TOOL_RESULT_START_TASK_INPUT_INVALID_FALLBACK_VAR_0??"the arguments"} ${TOOL_RESULT_START_TASK_INPUT_INVALID_FALLBACK_VAR_1.message??"are not valid"}
