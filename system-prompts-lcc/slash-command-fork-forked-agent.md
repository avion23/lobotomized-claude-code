<!--
name: 'Slash Command: /fork — forked agent'
description: >-
  /fork, /subtask and /btw fork result naming the forked agent and the last four
  characters of its id.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_FORK_FORKED_AGENT_VAR_0
  - SLASH_COMMAND_FORK_FORKED_AGENT_VAR_1
-->
${SLASH_COMMAND_FORK_FORKED_AGENT_VAR_0} forked ${SLASH_COMMAND_FORK_FORKED_AGENT_VAR_1.name} (${SLASH_COMMAND_FORK_FORKED_AGENT_VAR_1.agentId.slice(-4)})
