<!--
name: 'Tool Result: workflow remote agent cloud session waiting for input'
description: >-
  Workflow agent({isolation:'remote'}) failure when the cloud session is parked
  on a permission prompt, question or dialog nothing on this machine can answer.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_WORKFLOW_REMOTE_AGENT_CLOUD_SESSION_NEEDS_INPUT_VAR_0
-->
Cloud session ${TOOL_RESULT_WORKFLOW_REMOTE_AGENT_CLOUD_SESSION_NEEDS_INPUT_VAR_0} is waiting for input that nothing on this machine can give (a permission prompt, a question, or some other dialog). If it is a permission prompt, make sure the cloud agent's allowed_tools cover the tool, or use a permission mode that doesn't prompt; if it is a question, tell the agent in its prompt not to ask one.
