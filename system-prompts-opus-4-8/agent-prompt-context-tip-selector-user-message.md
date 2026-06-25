<!--
name: 'Agent Prompt: Context Tip Selector User Message'
description: >-
  User-message wrapper template for the context-tip selector call: transcript
  head plus <eligible_ids> and <transcript> blocks the model reads to pick a
  tip.
ccVersion: 2.1.191
variables:
  - AGENT_PROMPT_CONTEXT_TIP_SELECTOR_USER_MESSAGE_VAR_0
  - AGENT_PROMPT_CONTEXT_TIP_SELECTOR_USER_MESSAGE_VAR_1
  - AGENT_PROMPT_CONTEXT_TIP_SELECTOR_USER_MESSAGE_VAR_2
  - AGENT_PROMPT_CONTEXT_TIP_SELECTOR_USER_MESSAGE_VAR_3
-->
${AGENT_PROMPT_CONTEXT_TIP_SELECTOR_USER_MESSAGE_VAR_0(AGENT_PROMPT_CONTEXT_TIP_SELECTOR_USER_MESSAGE_VAR_1)}

<eligible_ids>${AGENT_PROMPT_CONTEXT_TIP_SELECTOR_USER_MESSAGE_VAR_2}</eligible_ids>

<transcript>
${AGENT_PROMPT_CONTEXT_TIP_SELECTOR_USER_MESSAGE_VAR_3}
</transcript>
