<!--
name: '/loop skill: decide-then-confirm steps (not yet armed)'
description: >-
  Numbered steps 3–4 of the /loop skill prompt for the not-yet-armed branch:
  decide first, then confirm after arming.
ccVersion: 2.1.284
variables:
  - SKILL_LOOP_STEPS_DECIDE_THEN_CONFIRM_VAR_0
  - SKILL_LOOP_STEPS_DECIDE_THEN_CONFIRM_VAR_1
  - SKILL_LOOP_STEPS_DECIDE_THEN_CONFIRM_VAR_2
-->
3. **Decide whether the loop continues.** ${SKILL_LOOP_STEPS_DECIDE_THEN_CONFIRM_VAR_0}
4. **After the wakeup is armed, briefly confirm**: ${SKILL_LOOP_STEPS_DECIDE_THEN_CONFIRM_VAR_1} you picked. ${SKILL_LOOP_STEPS_DECIDE_THEN_CONFIRM_VAR_2}
