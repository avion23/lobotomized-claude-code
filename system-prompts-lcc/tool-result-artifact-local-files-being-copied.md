<!--
name: 'Tool Result: artifact local — … local files being copied …….'
description: >-
  Piece of the model-facing text built beside
  tool-result-artifact-local-files-mixed-user-must-approve: "
  ${.length===2?"Both":`All ${.length}`} local files being copied
  ${.many}${(.group)}.". Emitted in the same string/return as that catalogued
  prompt.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_LOCAL_FILES_BEING_COPIED_VAR_0
  - TOOL_RESULT_ARTIFACT_LOCAL_FILES_BEING_COPIED_VAR_1
  - TOOL_RESULT_ARTIFACT_LOCAL_FILES_BEING_COPIED_VAR_2
-->
 ${TOOL_RESULT_ARTIFACT_LOCAL_FILES_BEING_COPIED_VAR_0.length===2?"Both":`All ${TOOL_RESULT_ARTIFACT_LOCAL_FILES_BEING_COPIED_VAR_0.length}`} local files being copied ${TOOL_RESULT_ARTIFACT_LOCAL_FILES_BEING_COPIED_VAR_1.many}${TOOL_RESULT_ARTIFACT_LOCAL_FILES_BEING_COPIED_VAR_2(TOOL_RESULT_ARTIFACT_LOCAL_FILES_BEING_COPIED_VAR_1.group)}.
