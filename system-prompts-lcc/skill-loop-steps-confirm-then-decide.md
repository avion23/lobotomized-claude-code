<!--
name: '/loop skill: confirm-then-decide steps (pre-armed)'
description: >-
  Numbered steps 3–4 of the /loop skill prompt for the pre-armed-wakeup branch:
  confirm the pick, then decide whether the loop continues.
ccVersion: 2.1.284
variables:
  - SKILL_LOOP_STEPS_CONFIRM_THEN_DECIDE_VAR_0
  - SKILL_LOOP_STEPS_CONFIRM_THEN_DECIDE_VAR_1
  - SKILL_LOOP_STEPS_CONFIRM_THEN_DECIDE_VAR_2
-->
3. **Briefly confirm**: ${SKILL_LOOP_STEPS_CONFIRM_THEN_DECIDE_VAR_0} you're about to pick. ${SKILL_LOOP_STEPS_CONFIRM_THEN_DECIDE_VAR_1}
4. **Then, as the last action of this turn, decide whether the loop continues.** ${SKILL_LOOP_STEPS_CONFIRM_THEN_DECIDE_VAR_2}
