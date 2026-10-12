<!--
name: 'ScheduleWakeup tool result: continue-instruction lead'
description: >-
  Lead sentence of the ScheduleWakeup tool result telling the model what to do
  (via Fln's per-mode phrasing) and to end the turn.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_SCHEDULEWAKEUP_CONTINUE_INSTRUCTION_LEAD_VAR_0
  - TOOL_RESULT_SCHEDULEWAKEUP_CONTINUE_INSTRUCTION_LEAD_VAR_1
-->
Then ${TOOL_RESULT_SCHEDULEWAKEUP_CONTINUE_INSTRUCTION_LEAD_VAR_0({briefMode:TOOL_RESULT_SCHEDULEWAKEUP_CONTINUE_INSTRUCTION_LEAD_VAR_1})} — and end the turn.
