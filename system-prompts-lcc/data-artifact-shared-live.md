<!--
name: 'Artifact: Classifier shared/live target state'
description: >-
  Classifier shared/live target state. Text emitted in the model permission
  classifier context.
ccVersion: 2.1.296
variables:
  - DATA_ARTIFACT_SHARED_LIVE_VAR_0
-->
 [shared-live: ${DATA_ARTIFACT_SHARED_LIVE_VAR_0.probeFailed?"unknown":DATA_ARTIFACT_SHARED_LIVE_VAR_0.mode}]
