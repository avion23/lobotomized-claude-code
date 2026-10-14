<!--
name: 'Tool Result: SendMessage agent stopped'
description: Says the agent was stopped by the user and not resumed; treat as cancelled
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_SEND_MESSAGE_AGENT_STOPPED_VAR_0
-->
Agent "${TOOL_RESULT_SEND_MESSAGE_AGENT_STOPPED_VAR_0}" was stopped by the user and was not resumed. Treat its work as cancelled; only start a new agent for it if the user explicitly asks.
