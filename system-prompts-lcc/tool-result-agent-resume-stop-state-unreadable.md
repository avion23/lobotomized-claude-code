<!--
name: Agent Resume Stop State Unreadable
description: >-
  Agent resume refusal clause: the agent's saved state cannot be read, so
  whether the user stopped it is unknown.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_AGENT_RESUME_STOP_STATE_UNREADABLE_VAR_0
  - TOOL_RESULT_AGENT_RESUME_STOP_STATE_UNREADABLE_VAR_1
  - TOOL_RESULT_AGENT_RESUME_STOP_STATE_UNREADABLE_VAR_2
  - TOOL_RESULT_AGENT_RESUME_STOP_STATE_UNREADABLE_VAR_3
-->
its saved state cannot be read (${TOOL_RESULT_AGENT_RESUME_STOP_STATE_UNREADABLE_VAR_0(TOOL_RESULT_AGENT_RESUME_STOP_STATE_UNREADABLE_VAR_1)??TOOL_RESULT_AGENT_RESUME_STOP_STATE_UNREADABLE_VAR_2(TOOL_RESULT_AGENT_RESUME_STOP_STATE_UNREADABLE_VAR_1)??"storage error"}), so it cannot be told whether the user stopped it. ${TOOL_RESULT_AGENT_RESUME_STOP_STATE_UNREADABLE_VAR_3?"Send the message again in a moment, or the user":"The user"} can resume it themselves.
