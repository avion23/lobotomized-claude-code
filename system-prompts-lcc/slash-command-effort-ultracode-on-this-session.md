<!--
name: '/effort ultracode toggle: on this session only'
description: >-
  Result message shown when ultracode is turned on for the current session only,
  confirming effort stays at the current level.
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_EFFORT_ULTRACODE_ON_THIS_SESSION_VAR_0
  - SLASH_COMMAND_EFFORT_ULTRACODE_ON_THIS_SESSION_VAR_1
  - SLASH_COMMAND_EFFORT_ULTRACODE_ON_THIS_SESSION_VAR_2
-->
Ultracode on (this session only): ${SLASH_COMMAND_EFFORT_ULTRACODE_ON_THIS_SESSION_VAR_0}. Effort stays ${SLASH_COMMAND_EFFORT_ULTRACODE_ON_THIS_SESSION_VAR_1}.${SLASH_COMMAND_EFFORT_ULTRACODE_ON_THIS_SESSION_VAR_2??""}
