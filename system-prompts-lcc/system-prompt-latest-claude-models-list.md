<!--
name: 'System Prompt: latest Claude models list'
description: >-
  Lists the most recent Claude model IDs and advises defaulting to the latest
  models when building AI apps
ccVersion: 2.1.301
variables:
  - SYSTEM_PROMPT_LATEST_CLAUDE_MODELS_LIST_VAR_0
-->
The most recent Claude models are as follows, with their model IDs: ${SYSTEM_PROMPT_LATEST_CLAUDE_MODELS_LIST_VAR_0.join(", ")}. When building AI applications, generally you want to use the latest and most capable Claude models by default.
