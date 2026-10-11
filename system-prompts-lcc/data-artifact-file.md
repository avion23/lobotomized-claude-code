<!--
name: 'Artifact: Classifier concealed source detail'
description: >-
  Classifier concealed source detail. Text emitted in the model permission
  classifier context.
ccVersion: 2.1.296
variables:
  - DATA_ARTIFACT_FILE_VAR_0
  - DATA_ARTIFACT_FILE_VAR_1
-->
 [file ${DATA_ARTIFACT_FILE_VAR_0}: ${[...DATA_ARTIFACT_FILE_VAR_1.hidden,...DATA_ARTIFACT_FILE_VAR_1.location].join("; ")}]
