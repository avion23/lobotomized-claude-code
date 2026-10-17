<!--
name: 'System Prompt: Cross-Session Messages Three Ways'
description: >-
  System-prompt clause describing three paths owner/member messages reach the
  agent, including in-thread sends.
ccVersion: 2.1.302
variables:
  - SYSTEM_PROMPT_CROSS_SESSION_MESSAGES_THREE_WAYS_VAR_0
-->
 Their messages reach the agent in three ways: the server attaches them to a coordinator session's relay, the server returns them from \`${SYSTEM_PROMPT_CROSS_SESSION_MESSAGES_THREE_WAYS_VAR_0.messages}\`, \`${SYSTEM_PROMPT_CROSS_SESSION_MESSAGES_THREE_WAYS_VAR_0.thread}\` and \`${SYSTEM_PROMPT_CROSS_SESSION_MESSAGES_THREE_WAYS_VAR_0.timeline}\`, and the person sends one in this thread (below).
