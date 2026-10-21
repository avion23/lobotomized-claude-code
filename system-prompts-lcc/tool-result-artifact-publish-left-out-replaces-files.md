<!--
name: 'Tool result: artifact publish left out, replaces files'
description: >-
  Publish refusal for a full-replace publish whose left-out copies could delete
  existing files.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_ARTIFACT_PUBLISH_LEFT_OUT_REPLACES_FILES_VAR_0
  - TOOL_RESULT_ARTIFACT_PUBLISH_LEFT_OUT_REPLACES_FILES_VAR_1
  - TOOL_RESULT_ARTIFACT_PUBLISH_LEFT_OUT_REPLACES_FILES_VAR_2
-->
${TOOL_RESULT_ARTIFACT_PUBLISH_LEFT_OUT_REPLACES_FILES_VAR_0}, and this publish replaces every file in the artifact, so publishing without the copies could delete a file it has. ${TOOL_RESULT_ARTIFACT_PUBLISH_LEFT_OUT_REPLACES_FILES_VAR_1} To save the rest, read the artifact to see which files it has, then publish again without the left-out copies. ${TOOL_RESULT_ARTIFACT_PUBLISH_LEFT_OUT_REPLACES_FILES_VAR_2}
