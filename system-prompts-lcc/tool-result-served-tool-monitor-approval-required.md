<!--
name: 'Tool result: served Monitor approval required'
description: >-
  Monitor run refusal when a person has to approve it first and the attached
  approval is not for this question.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_SERVED_TOOL_MONITOR_APPROVAL_REQUIRED_VAR_0
  - TOOL_RESULT_SERVED_TOOL_MONITOR_APPROVAL_REQUIRED_VAR_1
-->
${TOOL_RESULT_SERVED_TOOL_MONITOR_APPROVAL_REQUIRED_VAR_0.name} was not run: a person has to approve it first, and the approval sent with it, if any, is not for this question. Check the Monitor again to have it asked. The check said: ${TOOL_RESULT_SERVED_TOOL_MONITOR_APPROVAL_REQUIRED_VAR_1.verdict.message}
