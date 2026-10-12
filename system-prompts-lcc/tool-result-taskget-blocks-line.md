<!--
name: 'TaskGet result: blocks line'
description: Line listing the tasks this task blocks in the TaskGet tool result.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_TASKGET_BLOCKS_LINE_VAR_0
  - TOOL_RESULT_TASKGET_BLOCKS_LINE_VAR_1
-->
Blocks: ${TOOL_RESULT_TASKGET_BLOCKS_LINE_VAR_0.blocks.map((TOOL_RESULT_TASKGET_BLOCKS_LINE_VAR_1)=>`#${TOOL_RESULT_TASKGET_BLOCKS_LINE_VAR_1}`).join(", ")}
