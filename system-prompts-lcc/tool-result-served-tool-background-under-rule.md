<!--
name: 'Tool Result: served tool run_in_background under a rule'
description: >-
  Served tool not run because a deny or ask rule names run_in_background; resend
  without it
ccVersion: 2.1.301
variables:
  - TOOL_RESULT_SERVED_TOOL_BACKGROUND_UNDER_RULE_VAR_0
-->
${TOOL_RESULT_SERVED_TOOL_BACKGROUND_UNDER_RULE_VAR_0.name} was not run: a deny or ask permission rule names run_in_background. Send the call again without it. If you did not set it, a hook of this session did: tell the user.
