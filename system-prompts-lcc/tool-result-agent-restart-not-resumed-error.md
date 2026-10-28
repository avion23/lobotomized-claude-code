<!--
name: 'Tool Result: Agent not resumed after restart (error)'
description: >-
  Agent tool error when an agent stopped at a container restart was not resumed,
  with the underlying reason
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AGENT_RESTART_NOT_RESUMED_ERROR_VAR_0
  - TOOL_RESULT_AGENT_RESTART_NOT_RESUMED_ERROR_VAR_1
-->
Agent ${TOOL_RESULT_AGENT_RESTART_NOT_RESUMED_ERROR_VAR_0} stopped when the container was restarted and was not resumed: ${TOOL_RESULT_AGENT_RESTART_NOT_RESUMED_ERROR_VAR_1.message}
