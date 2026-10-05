<!--
name: 'Tool Result: Snooze send status update via brief tool'
description: >-
  Branch telling the agent to send the owed status update through the brief tool
  as proactive, since plain text counts as unread.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_SNOOZE_SEND_STATUS_UPDATE_VIA_BRIEF_VAR_0
-->
send it now via ${TOOL_RESULT_SNOOZE_SEND_STATUS_UPDATE_VIA_BRIEF_VAR_0} (\`status: 'proactive'\`) — plain response text is treated as unread in this session
