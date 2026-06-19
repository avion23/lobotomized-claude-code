<!--
name: 'System Prompt: Async agent launched result'
description: >-
  Tool_result confirming an async agent launched in the background, giving the
  internal agentId and SendMessage continuation hint
ccVersion: 2.1.178
variables:
  - SYSTEM_PROMPT_ASYNC_AGENT_LAUNCHED_RESULT_VAR_0
-->
Async agent launched successfully.
agentId: ${SYSTEM_PROMPT_ASYNC_AGENT_LAUNCHED_RESULT_VAR_0.agentId} (internal ID - do not mention to user. Use SendMessage with to: '${SYSTEM_PROMPT_ASYNC_AGENT_LAUNCHED_RESULT_VAR_0.agentId}' to continue this agent.)
The agent is working in the background. You will be notified automatically when it completes.
