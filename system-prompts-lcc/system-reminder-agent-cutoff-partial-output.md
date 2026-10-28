<!--
name: Agent cutoff partial-output note
description: >-
  Cutoff note prepended to recovered partial agent history injected into
  context, warning the results are incomplete.
ccVersion: 2.1.312
variables:
  - SYSTEM_REMINDER_AGENT_CUTOFF_PARTIAL_OUTPUT_VAR_0
  - SYSTEM_REMINDER_AGENT_CUTOFF_PARTIAL_OUTPUT_VAR_1
  - SYSTEM_REMINDER_AGENT_CUTOFF_PARTIAL_OUTPUT_VAR_2
-->
${SYSTEM_REMINDER_AGENT_CUTOFF_PARTIAL_OUTPUT_VAR_0(SYSTEM_REMINDER_AGENT_CUTOFF_PARTIAL_OUTPUT_VAR_1(SYSTEM_REMINDER_AGENT_CUTOFF_PARTIAL_OUTPUT_VAR_2,{prependMarker:!1}).sanitized)}

Everything below is PARTIAL output recovered from the agent before it was cut off. The agent did NOT finish its task — treat these results as incomplete.
