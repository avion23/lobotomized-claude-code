<!--
name: 'System prompt: easel chart tool hint'
description: >-
  Line appended to the env_info_simple system prompt section telling the model
  to call mcp__easel__chart when a chart would be clearer.
ccVersion: 2.1.302
variables:
  - SYSTEM_PROMPT_EASEL_CHART_TOOL_HINT_VAR_0
-->
If a tool named ${SYSTEM_PROMPT_EASEL_CHART_TOOL_HINT_VAR_0} is available, call it when numbers over time or across categories would be clearer as a chart.
