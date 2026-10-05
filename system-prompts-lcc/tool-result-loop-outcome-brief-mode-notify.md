<!--
name: 'Loop outcome: brief-mode notify instruction'
description: >-
  Brief-mode branch of Fln(), confirmed embedded in `k(){return `Then
  ${Fln(...)} — a stopped loop has no next tick to surface it.`}` used in the
  loop/wakeup tool description.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_LOOP_OUTCOME_BRIEF_MODE_NOTIFY_VAR_0
-->
send the loop's outcome to the user via ${TOOL_RESULT_LOOP_OUTCOME_BRIEF_MODE_NOTIFY_VAR_0} (\`status: 'proactive'\`) — plain response text is treated as unread in this session
