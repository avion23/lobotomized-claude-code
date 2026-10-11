<!--
name: 'TaskGet result: blocked-by line'
description: Line listing the tasks blocking this task in the TaskGet tool result.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_TASKGET_BLOCKED_BY_LINE_VAR_0
  - TOOL_RESULT_TASKGET_BLOCKED_BY_LINE_VAR_1
-->
Blocked by: ${TOOL_RESULT_TASKGET_BLOCKED_BY_LINE_VAR_0.blockedBy.map((TOOL_RESULT_TASKGET_BLOCKED_BY_LINE_VAR_1)=>`#${TOOL_RESULT_TASKGET_BLOCKED_BY_LINE_VAR_1}`).join(", ")}
