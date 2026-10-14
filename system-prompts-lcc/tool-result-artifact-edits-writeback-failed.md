<!--
name: 'Tool Result: Artifact edits write-back failed'
description: >-
  Warns the local file may be partly written after publish and asks to restore
  it before republishing
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_FAILED_VAR_0
  - TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_FAILED_VAR_1
  - TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_FAILED_VAR_2
  - TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_FAILED_VAR_3
-->
${TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_FAILED_VAR_0}: writing it back failed, and the file may be partly written. Read it before anything else, restore it to the published text (${TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_FAILED_VAR_1}, ${TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_FAILED_VAR_2?"the edit":"the edits"} included), and only then publish it again; publishing it as it is could put damaged content ${TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_FAILED_VAR_3==="page"?"on the page":"in the artifact"}.
