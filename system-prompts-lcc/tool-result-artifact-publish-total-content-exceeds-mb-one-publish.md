<!--
name: 'Artifact publish: total content exceeds per-publish MB limit'
description: >-
  Error returned from Artifact publish validation when the combined byte size of
  files in one publish call exceeds the per-publish cap.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_PUBLISH_TOTAL_CONTENT_EXCEEDS_MB_ONE_PUBLISH_VAR_0
  - TOOL_RESULT_ARTIFACT_PUBLISH_TOTAL_CONTENT_EXCEEDS_MB_ONE_PUBLISH_VAR_1
  - TOOL_RESULT_ARTIFACT_PUBLISH_TOTAL_CONTENT_EXCEEDS_MB_ONE_PUBLISH_VAR_2
  - TOOL_RESULT_ARTIFACT_PUBLISH_TOTAL_CONTENT_EXCEEDS_MB_ONE_PUBLISH_VAR_3
-->
total content is ${TOOL_RESULT_ARTIFACT_PUBLISH_TOTAL_CONTENT_EXCEEDS_MB_ONE_PUBLISH_VAR_0.ceil(TOOL_RESULT_ARTIFACT_PUBLISH_TOTAL_CONTENT_EXCEEDS_MB_ONE_PUBLISH_VAR_1/1024/1024)}MB — one publish may send at most ${TOOL_RESULT_ARTIFACT_PUBLISH_TOTAL_CONTENT_EXCEEDS_MB_ONE_PUBLISH_VAR_2/1024/1024}MB. Nothing was published: send part of the files now and the rest with another publish to the same url (files left out of a later publish are kept; a version may total ${TOOL_RESULT_ARTIFACT_PUBLISH_TOTAL_CONTENT_EXCEEDS_MB_ONE_PUBLISH_VAR_3/1024/1024}MB).
