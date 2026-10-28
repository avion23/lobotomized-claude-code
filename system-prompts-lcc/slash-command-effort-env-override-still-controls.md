<!--
name: 'Slash Command: /effort env override still controls'
description: >-
  /effort result when CLAUDE_CODE_EFFORT_LEVEL still controls the session after
  clearing or setting effort
ccVersion: 2.1.312
variables:
  - SLASH_COMMAND_EFFORT_ENV_OVERRIDE_STILL_CONTROLS_VAR_0
  - SLASH_COMMAND_EFFORT_ENV_OVERRIDE_STILL_CONTROLS_VAR_1
  - SLASH_COMMAND_EFFORT_ENV_OVERRIDE_STILL_CONTROLS_VAR_2
-->
${SLASH_COMMAND_EFFORT_ENV_OVERRIDE_STILL_CONTROLS_VAR_0?"Cleared effort from settings, but":`Effort set to ${SLASH_COMMAND_EFFORT_ENV_OVERRIDE_STILL_CONTROLS_VAR_1()} for this session, but`} CLAUDE_CODE_EFFORT_LEVEL=${SLASH_COMMAND_EFFORT_ENV_OVERRIDE_STILL_CONTROLS_VAR_2} still controls this session
