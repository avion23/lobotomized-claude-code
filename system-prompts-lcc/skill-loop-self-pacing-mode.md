<!--
name: 'Skill: /loop self-pacing mode'
description: >-
  Instructs Claude how to self-pace a recurring loop by arming event monitors as
  primary wake signals and scheduling fallback heartbeat delays between
  iterations
ccVersion: 2.1.284
variables:
  - MONITOR_TOOL_NAME
  - MONITOR_ARMING_GUIDANCE_FN
  - SCHEDULE_WAKEUP_TOOL_NAME
  - MONITOR_REARM_GUIDANCE_FN
  - LOOP_CONFIRM_AND_DECIDE_STEPS
  - REARM_UPDATE_ORDER_FN
  - TASK_STOP_TOOL_NAME
  - TASK_LIST_TOOL_NAME
  - LOOP_OUTCOME_REPORT_FN
  - ADDITIONAL_INFO_FN
-->
The user wants you to self-pace. Decide what makes the next iteration worth running — a passage of time, or an observable event.

1. **Run the parsed prompt now.** If it's a slash command, invoke it via the Skill tool; otherwise act on it directly.
2. **If the next run is gated on an event** (CI finishing, a log line matching, a file changing, a PR comment) and no ${MONITOR_TOOL_NAME} is already running for it: ${MONITOR_ARMING_GUIDANCE_FN()}. Its events arrive as \`<task-notification>\` messages and wake this loop immediately — you don't wait for the ${SCHEDULE_WAKEUP_TOOL_NAME} deadline. ${MONITOR_REARM_GUIDANCE_FN("iterations")}
${LOOP_CONFIRM_AND_DECIDE_STEPS}
5. **If woken by a \`<task-notification>\`** rather than this prompt: handle the event in the context of the loop task, then make the same continue-or-stop decision. To continue, ${REARM_UPDATE_ORDER_FN(`call ${SCHEDULE_WAKEUP_TOOL_NAME} again with the same \`prompt\` and the same 1200–1800s \`delaySeconds\` from the schedule step above (the ${MONITOR_TOOL_NAME} remains the wake signal; the new wakeup is only the fallback heartbeat)`)}. If the event means the work is done, stop (step 6).
6. **To stop the loop** — task complete, no further progress possible, or the user asked — call ${SCHEDULE_WAKEUP_TOOL_NAME} with \`stop: true\` (no other fields) and ${TASK_STOP_TOOL_NAME} any ${MONITOR_TOOL_NAME} you armed (use ${TASK_LIST_TOOL_NAME} to find the task ID if it's no longer in context).${LOOP_OUTCOME_REPORT_FN()}${ADDITIONAL_INFO_FN()}
