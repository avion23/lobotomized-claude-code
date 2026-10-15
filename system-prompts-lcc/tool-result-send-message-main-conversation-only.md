<!--
name: 'Tool Result: SendMessage unavailable in this session'
description: >-
  Not sent: SendMessage is switched off for subagents or the caller was stopped;
  pass info in the final response
ccVersion: 2.1.301
variables:
  - TOOL_RESULT_SEND_MESSAGE_MAIN_CONVERSATION_ONLY_VAR_0
-->
Not sent. You cannot use ${TOOL_RESULT_SEND_MESSAGE_MAIN_CONVERSATION_ONLY_VAR_0} in this session: it is switched off for subagents, or you were stopped. Put what you need to pass on in your final response, which goes to whoever launched or resumed you.
