<!--
name: 'System reminder: output token usage per turn and session'
description: >-
  Meta attachment telling the model output tokens spent this turn (against any
  budget) and across the session.
ccVersion: 2.1.296
variables:
  - SYSTEM_REMINDER_OUTPUT_TOKEN_USAGE_TURN_SESSION_VAR_0
  - SYSTEM_REMINDER_OUTPUT_TOKEN_USAGE_TURN_SESSION_VAR_1
  - SYSTEM_REMINDER_OUTPUT_TOKEN_USAGE_TURN_SESSION_VAR_2
-->
Output tokens — turn: ${SYSTEM_REMINDER_OUTPUT_TOKEN_USAGE_TURN_SESSION_VAR_0} · session: ${SYSTEM_REMINDER_OUTPUT_TOKEN_USAGE_TURN_SESSION_VAR_1(SYSTEM_REMINDER_OUTPUT_TOKEN_USAGE_TURN_SESSION_VAR_2.session)}
