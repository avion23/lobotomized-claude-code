<!--
name: 'ScheduleWakeup tool result: rearm-if-armed suffix'
description: >-
  Suffix appended to the ScheduleWakeup tool result reminding the model to
  re-arm any snooze it had set for the loop, when the loop is stopping.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_LOOP_REARM_SUFFIX_VAR_0
  - TOOL_RESULT_LOOP_REARM_SUFFIX_VAR_1
  - TOOL_RESULT_LOOP_REARM_SUFFIX_VAR_2
-->
If you armed a ${TOOL_RESULT_LOOP_REARM_SUFFIX_VAR_0} for this loop, ${TOOL_RESULT_LOOP_REARM_SUFFIX_VAR_1} it now. ${TOOL_RESULT_LOOP_REARM_SUFFIX_VAR_2}
