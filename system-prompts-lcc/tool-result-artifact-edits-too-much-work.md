<!--
name: 'Tool Result: Artifact edits too many per call'
description: >-
  Rejects an Artifact publish carrying more edits than one call applies for the
  file size and gives the per-call limit
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_0
  - TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_1
  - TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_2
  - TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_3
-->
${TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_0} edits on a file of ${TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_1} characters is more than one publish call will apply; send at most ${TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_2.max(1,TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_2.floor(TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_3/TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_2.max(1,TOOL_RESULT_ARTIFACT_EDITS_TOO_MUCH_WORK_VAR_1)))} edits per call for a file this size, over as many calls as the change needs
