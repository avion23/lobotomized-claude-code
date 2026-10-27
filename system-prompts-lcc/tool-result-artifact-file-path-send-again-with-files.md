<!--
name: Artifact send again with files
description: Clause telling Claude to resend with a files entry
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_ARTIFACT_FILE_PATH_SEND_AGAIN_WITH_FILES_VAR_0
-->
send the call again ${TOOL_RESULT_ARTIFACT_FILE_PATH_SEND_AGAIN_WITH_FILES_VAR_0.edits?"without `edits` (make the change in the file first) and ":""}with ${TOOL_RESULT_ARTIFACT_FILE_PATH_SEND_AGAIN_WITH_FILES_VAR_0.files==="none"?"this entry in `files`":TOOL_RESULT_ARTIFACT_FILE_PATH_SEND_AGAIN_WITH_FILES_VAR_0.files==="map"?"this entry added to `files`":"`files` as a map that states each file's served path, with this entry added"}:
