<!--
name: 'Tool result: workflow agent bashCommandClamp on Bash-less agent (lead)'
description: >-
  Lead fragment of the workflow agent() refusal when bashCommandClamp is set but
  the spawned agent's tool pool has no Bash.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_WORKFLOW_AGENT_BASH_COMMAND_CLAMP_BASHLESS_AGENT_LEAD_VAR_0
-->
agent() opts.bashCommandClamp can bind nothing: the spawned agent's resolved tool pool has no ${TOOL_RESULT_WORKFLOW_AGENT_BASH_COMMAND_CLAMP_BASHLESS_AGENT_LEAD_VAR_0} (removed by this spawn's disallowedTools, the agent definition's denies, or absent from the session pool). A clamp on a Bash-less agent 
