<!--
name: 'Artifact: Classifier named thumbnails'
description: >-
  Classifier named thumbnails. Text emitted in the model permission classifier
  context.
ccVersion: 2.1.296
variables:
  - DATA_ARTIFACT_THUMBNAIL_VAR_0
  - DATA_ARTIFACT_THUMBNAIL_VAR_1
-->
(+thumbnail: ${DATA_ARTIFACT_THUMBNAIL_VAR_0.map(DATA_ARTIFACT_THUMBNAIL_VAR_1).join(", ")})
