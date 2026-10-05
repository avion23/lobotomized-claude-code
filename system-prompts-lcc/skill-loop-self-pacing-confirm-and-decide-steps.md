<!--
name: 'Skill: Loop self-pacing confirm and decide steps'
description: >-
  Steps 3-4 block of the self-pacing loop mode: when to call ScheduleWakeup
  again, the fallback-heartbeat delay with an armed Monitor, and the reason
  field.
ccVersion: 2.1.284
variables:
  - SKILL_LOOP_SELF_PACING_CONFIRM_AND_DECIDE_STEPS_VAR_0
  - SKILL_LOOP_SELF_PACING_CONFIRM_AND_DECIDE_STEPS_VAR_1
-->
If the task needs another iteration, call ${SKILL_LOOP_SELF_PACING_CONFIRM_AND_DECIDE_STEPS_VAR_0} with:
   - \`delaySeconds\`: with a ${SKILL_LOOP_SELF_PACING_CONFIRM_AND_DECIDE_STEPS_VAR_1} armed this is the **fallback heartbeat** — how long to wait if no event fires (lean 1200–1800s; idle ticks more frequent than the task needs are pure overhead). Without a ${SKILL_LOOP_SELF_PACING_CONFIRM_AND_DECIDE_STEPS_VAR_1} this is the cadence — pick based on what you observed. Read the tool's own description for cache-aware delay guidance.
   - \`reason\`: one short sentence on why you picked that delay.
   - \`prompt\`: the full original /loop input verbatim, prefixed with \`/loop \` so the next firing re-enters this skill and continues the loop. For example, if the user typed \`/loop check the deploy\`, pass \`/loop check the deploy\` as the prompt.
   - \`noop\`: \`true\` if this tick changed nothing ("still waiting", "quiet hold"); \`false\` if it did something worth keeping. Consecutive \`noop: true\` ticks collapse in the terminal.
   If it doesn't need another iteration, stop instead (step 6) — re-arming is a per-turn choice, not a default.
