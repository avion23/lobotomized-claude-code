<!--
name: 'Tool Result: cloud session not finished starting'
description: >-
  Refusal text for a cloud-session/remote-devices tool call made before that
  machine's Claude Code finished loading hooks and settings; instructs telling
  the user if it recurs.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_CLOUD_SESSION_NOT_FINISHED_STARTING_VAR_0
-->
Claude Code on ${TOOL_RESULT_CLOUD_SESSION_NOT_FINISHED_STARTING_VAR_0} has only just started and had not finished loading the hooks and settings it checks every call against before this call's time ran out — nothing ran. Send the call again in a moment. If it is refused this way again, tell the user that Claude Code on ${TOOL_RESULT_CLOUD_SESSION_NOT_FINISHED_STARTING_VAR_0} is not finishing its start-up.
