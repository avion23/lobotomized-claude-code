<!--
name: 'Tool Result: ScheduleWakeup only-tool-call status update timing'
description: >-
  Tells Claude that when ScheduleWakeup is its only tool call this turn, the
  turn ends immediately when it returns, so any status update must be sent
  before calling it, and to end the turn now if reading this mid-turn.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_SCHEDULEWAKEUP_ONLY_TOOL_CALL_STATUS_UPDATE_TIMING_VAR_0
  - TOOL_RESULT_SCHEDULEWAKEUP_ONLY_TOOL_CALL_STATUS_UPDATE_TIMING_VAR_1
  - TOOL_RESULT_SCHEDULEWAKEUP_ONLY_TOOL_CALL_STATUS_UPDATE_TIMING_VAR_2
-->
When this call is your only tool call, the turn ends when it returns — there is no post-arm slot for a status update, so ${TOOL_RESULT_SCHEDULEWAKEUP_ONLY_TOOL_CALL_STATUS_UPDATE_TIMING_VAR_0?`send the per-tick update via ${TOOL_RESULT_SCHEDULEWAKEUP_ONLY_TOOL_CALL_STATUS_UPDATE_TIMING_VAR_1} (\`status: 'proactive'\`)`:"write the per-tick update as ordinary response text"} immediately BEFORE calling ${TOOL_RESULT_SCHEDULEWAKEUP_ONLY_TOOL_CALL_STATUS_UPDATE_TIMING_VAR_2}. If you are reading this mid-turn, end the turn now — the harness re-invokes you when the wakeup fires or a task-notification arrives.
