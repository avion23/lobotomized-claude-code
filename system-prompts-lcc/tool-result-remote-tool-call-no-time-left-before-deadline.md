<!--
name: Call reached target with no time left before deadline
description: >-
  tool_result message when a call reaches the target with no time left before
  its admission deadline because admission took longer than the caller allowed.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_CALL_NO_TIME_LEFT_BEFORE_DEADLINE_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_CALL_NO_TIME_LEFT_BEFORE_DEADLINE_VAR_1
  - TOOL_RESULT_REMOTE_TOOL_CALL_NO_TIME_LEFT_BEFORE_DEADLINE_VAR_2
  - TOOL_RESULT_REMOTE_TOOL_CALL_NO_TIME_LEFT_BEFORE_DEADLINE_VAR_3
-->
The call reached ${TOOL_RESULT_REMOTE_TOOL_CALL_NO_TIME_LEFT_BEFORE_DEADLINE_VAR_0.targetName} with no time left before its ${TOOL_RESULT_REMOTE_TOOL_CALL_NO_TIME_LEFT_BEFORE_DEADLINE_VAR_1(TOOL_RESULT_REMOTE_TOOL_CALL_NO_TIME_LEFT_BEFORE_DEADLINE_VAR_2.max(1000,TOOL_RESULT_REMOTE_TOOL_CALL_NO_TIME_LEFT_BEFORE_DEADLINE_VAR_3))} deadline (admission took longer than the caller allowed) — nothing ran.
