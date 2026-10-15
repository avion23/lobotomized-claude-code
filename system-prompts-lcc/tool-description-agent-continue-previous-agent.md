<!--
name: 'Tool Description: Agent continue previous agent'
description: >-
  Use the continue tool with an agent ID or name to resume it with context; a
  new call starts fresh
ccVersion: 2.1.301
variables:
  - TOOL_DESCRIPTION_AGENT_CONTINUE_PREVIOUS_AGENT_VAR_0
  - TOOL_DESCRIPTION_AGENT_CONTINUE_PREVIOUS_AGENT_VAR_1
  - TOOL_DESCRIPTION_AGENT_CONTINUE_PREVIOUS_AGENT_VAR_2
-->
You can use ${TOOL_DESCRIPTION_AGENT_CONTINUE_PREVIOUS_AGENT_VAR_0} with the agent's ID or name to continue a previously-spawned agent with its context still intact, whereas a new ${TOOL_DESCRIPTION_AGENT_CONTINUE_PREVIOUS_AGENT_VAR_1} call starts fresh${TOOL_DESCRIPTION_AGENT_CONTINUE_PREVIOUS_AGENT_VAR_2?" (except for fork types, which inherit your context)":""}.
