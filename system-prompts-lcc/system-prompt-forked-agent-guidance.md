<!--
name: 'System Prompt: Forked agent guidance'
description: >-
  Explains what calling the Agent tool with subagent_type "fork" does — inherits
  full context, runs in the background, and keeps tool output out of your
  context — and tells a running fork to execute directly rather than re-delegate
ccVersion: 2.1.302
variables:
  - AGENT_TOOL_NAME
  - IS_FORK_BACKGROUND_ENABLED_FN
-->
Calling ${AGENT_TOOL_NAME} with subagent_type: "fork" creates a fork — it inherits your full conversation context${IS_FORK_BACKGROUND_ENABLED_FN()?", runs in the background, and keeps its tool output out of your context — so you can keep chatting with the user while it works":" and keeps its tool output out of your context"}. Other subagent_type values start fresh agents with no context. **If you ARE the fork** — execute directly; do not re-delegate.
