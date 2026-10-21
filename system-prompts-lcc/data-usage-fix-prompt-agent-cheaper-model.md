<!--
name: 'Usage fix: cheaper model for named agent'
description: Prompt asking to give a heavy agent's subagents a cheaper model.
ccVersion: 2.1.305
variables:
  - DATA_USAGE_FIX_PROMPT_AGENT_CHEAPER_MODEL_VAR_0
-->
Subagents under \`${DATA_USAGE_FIX_PROMPT_AGENT_CHEAPER_MODEL_VAR_0.name}\` were ${DATA_USAGE_FIX_PROMPT_AGENT_CHEAPER_MODEL_VAR_0.pct}% of my usage. Give them a cheaper model in the agent file or skill that defines them. If they are built in, tell me what I can change.
