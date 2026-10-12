<!--
name: >-
  Data: Artifact upload_asset list auto-classifier — also names file_path, and a
  call naming both is refused
description: >-
  Classifier-input clause noting the call also names `file_path` and that a call
  naming both `file_path` and `file_paths` is refused.
ccVersion: 2.1.296
variables:
  - DATA_ARTIFACT_UPLOAD_ASSET_LIST_ALSO_NAMES_FILE_PATH_REFUSED_VAR_0
  - DATA_ARTIFACT_UPLOAD_ASSET_LIST_ALSO_NAMES_FILE_PATH_REFUSED_VAR_1
-->
; also names \`file_path\`${typeof DATA_ARTIFACT_UPLOAD_ASSET_LIST_ALSO_NAMES_FILE_PATH_REFUSED_VAR_0.file_path==="string"?` ${DATA_ARTIFACT_UPLOAD_ASSET_LIST_ALSO_NAMES_FILE_PATH_REFUSED_VAR_1.quote(DATA_ARTIFACT_UPLOAD_ASSET_LIST_ALSO_NAMES_FILE_PATH_REFUSED_VAR_0.file_path)}`:""}, and a call naming both is refused
