<!--
name: '/loop skill: stopped-loop next-tick note'
description: >-
  Note in the /loop skill prompt reminding the model to confirm before stopping
  since a stopped loop has no future tick.
ccVersion: 2.1.284
variables:
  - SKILL_LOOP_STOP_NO_NEXT_TICK_NOTE_VAR_0
  - SKILL_LOOP_STOP_NO_NEXT_TICK_NOTE_VAR_1
-->
 Then ${SKILL_LOOP_STOP_NO_NEXT_TICK_NOTE_VAR_0({briefMode:SKILL_LOOP_STOP_NO_NEXT_TICK_NOTE_VAR_1()})} — a stopped loop has no next tick to surface it.
