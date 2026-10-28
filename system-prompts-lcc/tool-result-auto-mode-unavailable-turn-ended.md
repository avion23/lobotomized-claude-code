<!--
name: 'Tool Result: Auto mode unavailable, turn ended'
description: >-
  Deny message when auto mode's safety check does not run or keeps giving no
  result, so the call was not run and the turn ends
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AUTO_MODE_UNAVAILABLE_TURN_ENDED_VAR_0
  - TOOL_RESULT_AUTO_MODE_UNAVAILABLE_TURN_ENDED_VAR_1
-->
Auto mode is unavailable: ${TOOL_RESULT_AUTO_MODE_UNAVAILABLE_TURN_ENDED_VAR_0===void 0?"its safety check does not run for this session":"its safety check keeps giving no result for this session's actions"}, so ${TOOL_RESULT_AUTO_MODE_UNAVAILABLE_TURN_ENDED_VAR_1.name} was not run and this turn has ended. Wait for the user's next message before doing anything further.
