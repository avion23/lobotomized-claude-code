<!--
name: 'Artifact permission ask: ''Let Claude …?'''
description: Permission ask question naming the action and source artifact.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_LET_CLAUDE_ASK_VAR_0
  - TOOL_RESULT_ARTIFACT_LET_CLAUDE_ASK_VAR_1
-->
Let Claude ${TOOL_RESULT_ARTIFACT_LET_CLAUDE_ASK_VAR_0(` from ${TOOL_RESULT_ARTIFACT_LET_CLAUDE_ASK_VAR_1.title!==void 0?`"${TOOL_RESULT_ARTIFACT_LET_CLAUDE_ASK_VAR_1.title}"`:"this artifact"}`)}?
