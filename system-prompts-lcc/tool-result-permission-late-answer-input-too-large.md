<!--
name: 'Tool Result: Late permission answer input too large'
description: >-
  Denial that a permission answer gave the call an input past the session's size
  bounds, so the call did not run
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_PERMISSION_LATE_ANSWER_INPUT_TOO_LARGE_VAR_0
  - TOOL_RESULT_PERMISSION_LATE_ANSWER_INPUT_TOO_LARGE_VAR_1
  - TOOL_RESULT_PERMISSION_LATE_ANSWER_INPUT_TOO_LARGE_VAR_2
-->
The call was not run. The permission answer gave it an input past what this session takes from an answer: ${TOOL_RESULT_PERMISSION_LATE_ANSWER_INPUT_TOO_LARGE_VAR_0} values, ${TOOL_RESULT_PERMISSION_LATE_ANSWER_INPUT_TOO_LARGE_VAR_1} levels of nesting, ${TOOL_RESULT_PERMISSION_LATE_ANSWER_INPUT_TOO_LARGE_VAR_2} characters of text. Nothing of the answer is in force.
