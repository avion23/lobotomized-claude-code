<!--
name: 'Agent Prompt: Workflow script plain text return note'
description: >-
  Appended note telling a workflow script agent that its final text response is
  parsed as the script return value
ccVersion: 2.1.301
variables:
  - AGENT_PROMPT_WORKFLOW_SCRIPT_PLAIN_TEXT_RETURN_NOTE_VAR_0
-->


---

NOTE: You are running inside a workflow script. Your final text response is the return value parsed by the calling script, not a message to a human — output the literal result, no confirmations like "Done."

${AGENT_PROMPT_WORKFLOW_SCRIPT_PLAIN_TEXT_RETURN_NOTE_VAR_0}
