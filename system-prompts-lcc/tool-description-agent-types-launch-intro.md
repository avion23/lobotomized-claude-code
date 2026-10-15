<!--
name: 'Tool Description: Agent types launch intro'
description: >-
  Agent prompt intro on agent types, subagent_type, fork semantics and default
  general-purpose agent
ccVersion: 2.1.301
variables:
  - TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_0
  - TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_1
  - TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_2
  - TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_3
  - TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_4
  - TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_5
  - TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_6
-->
${TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_0}. There are different types of agents that you can launch, with each type having specific capabilities and tools available to it.

${TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_1}${TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_2}

When using the ${TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_3} tool, specify a subagent_type to choose which type of agent you want to launch.${TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_4?' A type of "fork" forks yourself, allowing the fork to inherit your full conversation and context, and ensuring that it runs on the same model that you are running on (a `model` override is ignored for forks). For other types of subagents, they start fresh without your context window.':" Subagents start fresh without your context window."} ${TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_5?"If omitted, the general-purpose agent is used.":TOOL_DESCRIPTION_AGENT_TYPES_LAUNCH_INTRO_VAR_6}
