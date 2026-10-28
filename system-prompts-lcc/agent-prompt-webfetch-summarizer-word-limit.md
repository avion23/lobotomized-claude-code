<!--
name: 'Agent Prompt: WebFetch summarizer word limit'
description: >-
  Clause capping the WebFetch summary at a word count and asking to note in one
  line anything left out
ccVersion: 2.1.311
variables:
  - AGENT_PROMPT_WEBFETCH_SUMMARIZER_WORD_LIMIT_VAR_0
-->
 - Keep the response under ${AGENT_PROMPT_WEBFETCH_SUMMARIZER_WORD_LIMIT_VAR_0} words. If that leaves out something that was asked for, say so in one line.
