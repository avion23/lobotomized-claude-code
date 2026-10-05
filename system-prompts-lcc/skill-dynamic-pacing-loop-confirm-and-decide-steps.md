<!--
name: 'Skill: Dynamic pacing loop confirm and decide steps'
description: >-
  Steps 3-4 block of the dynamic-pacing loop skill: when to call ScheduleWakeup
  again, how to pick delaySeconds with or without an armed Monitor, and the
  reason field.
ccVersion: 2.1.284
variables:
  - SKILL_DYNAMIC_PACING_LOOP_CONFIRM_AND_DECIDE_STEPS_VAR_0
  - SKILL_DYNAMIC_PACING_LOOP_CONFIRM_AND_DECIDE_STEPS_VAR_1
  - SKILL_DYNAMIC_PACING_LOOP_CONFIRM_AND_DECIDE_STEPS_VAR_2
-->
If the next check is worth running, call ${SKILL_DYNAMIC_PACING_LOOP_CONFIRM_AND_DECIDE_STEPS_VAR_0} with:
   - \`delaySeconds\`: with a ${SKILL_DYNAMIC_PACING_LOOP_CONFIRM_AND_DECIDE_STEPS_VAR_1} armed this is the fallback heartbeat (lean 1200–1800s). Without one, pick based on what you observed this turn — quiet branch? wait longer. Lots in flight? wait shorter. Read the tool's own description for cache-aware delay guidance.
   - \`reason\`: one short sentence on why you picked that delay.
   - \`prompt\`: the literal string \`${SKILL_DYNAMIC_PACING_LOOP_CONFIRM_AND_DECIDE_STEPS_VAR_2}\` — the dynamic-mode sentinel expands at fire time to the full instructions (first fire / first fire post-compact / loop.md edited) or a dynamic-pacing-specific short reminder (subsequent fires). Do not pass the full instructions; that is handled automatically.
   - \`noop\`: \`true\` if this tick changed nothing ("still waiting", "quiet hold"); \`false\` if it did something worth keeping. Consecutive \`noop: true\` ticks collapse in the terminal.
   If it isn't, stop instead (step 6) — re-arming is a per-turn choice, not a default.
