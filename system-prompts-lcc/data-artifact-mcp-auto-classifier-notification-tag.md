<!--
name: 'Data: Artifacts MCP classifier notification tag'
description: >-
  Tag added to the auto-mode classifier input marking a call requested after a
  new-comments notification, noting that viewer-written rows or comments are
  ingested
ccVersion: 2.1.310
variables:
  - DATA_ARTIFACT_MCP_AUTO_CLASSIFIER_NOTIFICATION_TAG_VAR_0
-->
 [requested after a new-comments notification${DATA_ARTIFACT_MCP_AUTO_CLASSIFIER_NOTIFICATION_TAG_VAR_0==="rows"?": rows are written by artifact viewers":DATA_ARTIFACT_MCP_AUTO_CLASSIFIER_NOTIFICATION_TAG_VAR_0==="comments"?": the comment text it ingests is written by artifact viewers":""}]
