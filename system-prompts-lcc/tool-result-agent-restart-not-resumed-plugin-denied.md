<!--
name: 'Tool Result: Agent not resumed after restart (plugin denied)'
description: >-
  Agent tool error when a plugin denied resuming an agent stopped at a container
  restart
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AGENT_RESTART_NOT_RESUMED_PLUGIN_DENIED_VAR_0
  - TOOL_RESULT_AGENT_RESTART_NOT_RESUMED_PLUGIN_DENIED_VAR_1
-->
Agent ${TOOL_RESULT_AGENT_RESTART_NOT_RESUMED_PLUGIN_DENIED_VAR_0} stopped when the container was restarted and was not resumed: ${TOOL_RESULT_AGENT_RESTART_NOT_RESUMED_PLUGIN_DENIED_VAR_1.deniedByPlugin}
