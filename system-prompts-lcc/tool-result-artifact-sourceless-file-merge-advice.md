<!--
name: Artifact Sourceless File Merge Advice
description: >-
  File-mode advice in a sourceless Artifact refusal: merge anything missing into
  the file, else send the publish again.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_ARTIFACT_SOURCELESS_FILE_MERGE_ADVICE_VAR_0
-->
 If your file leaves out anything in that version, merge it into your file with Edit or Write, ${TOOL_RESULT_ARTIFACT_SOURCELESS_FILE_MERGE_ADVICE_VAR_0}; if your file itself genuinely already holds that version's changes, send the publish again and it will go through unless the artifact changes again first.
