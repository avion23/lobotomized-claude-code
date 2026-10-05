<!--
name: 'Tool Result: remote-tool call needs approval'
description: >-
  Text returned as the tool_result content when a call routed to an attached
  machine/remote tool is pending an approval decision in this session
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_APPROVAL_NEEDED_ELICITATION_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_APPROVAL_NEEDED_ELICITATION_VAR_1
-->
${TOOL_RESULT_REMOTE_TOOL_APPROVAL_NEEDED_ELICITATION_VAR_0.toolName} on ${TOOL_RESULT_REMOTE_TOOL_APPROVAL_NEEDED_ELICITATION_VAR_0.target.name} needs approval in this session before it runs: ${TOOL_RESULT_REMOTE_TOOL_APPROVAL_NEEDED_ELICITATION_VAR_1}
