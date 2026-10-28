<!--
name: Artifact updated unchanged files
description: Note listing files already in the Artifact with the same content
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_ARTIFACT_UPDATED_UNCHANGED_FILES_NOTE_VAR_0
  - TOOL_RESULT_ARTIFACT_UPDATED_UNCHANGED_FILES_NOTE_VAR_1
-->
 Already in the Artifact with the same content, so not changed by this publish: ${TOOL_RESULT_ARTIFACT_UPDATED_UNCHANGED_FILES_NOTE_VAR_0(TOOL_RESULT_ARTIFACT_UPDATED_UNCHANGED_FILES_NOTE_VAR_1)}. If you meant to change ${TOOL_RESULT_ARTIFACT_UPDATED_UNCHANGED_FILES_NOTE_VAR_1.length===1?"it, check the local file":"one of them, check the local files"} you sent: if your change is missing there, make it and publish again; if it is there, the Artifact already has it.
