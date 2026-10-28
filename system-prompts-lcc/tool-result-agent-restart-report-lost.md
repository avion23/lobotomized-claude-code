<!--
name: 'Tool Result: Agent report lost in container restart'
description: >-
  Agent tool error when the agent had finished but its report was lost when the
  container restarted
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AGENT_RESTART_REPORT_LOST_VAR_0
-->
Agent ${TOOL_RESULT_AGENT_RESTART_REPORT_LOST_VAR_0} had finished when the container was restarted, but its report was lost with the restart. It was not run again. Send it a message to ask for its report.
