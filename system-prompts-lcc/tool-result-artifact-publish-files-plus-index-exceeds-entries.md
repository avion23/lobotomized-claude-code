<!--
name: 'Artifact publish: files count plus index.html exceeds limit'
description: >-
  Validation error when the files map plus the implicit index.html entry exceeds
  the max entries one publish call may name.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_PUBLISH_FILES_PLUS_INDEX_EXCEEDS_ENTRIES_VAR_0
  - TOOL_RESULT_ARTIFACT_PUBLISH_FILES_PLUS_INDEX_EXCEEDS_ENTRIES_VAR_1
-->
files: ${TOOL_RESULT_ARTIFACT_PUBLISH_FILES_PLUS_INDEX_EXCEEDS_ENTRIES_VAR_0.length} files + index.html exceeds the ${TOOL_RESULT_ARTIFACT_PUBLISH_FILES_PLUS_INDEX_EXCEEDS_ENTRIES_VAR_1+1} entries one publish may name; send at most ${TOOL_RESULT_ARTIFACT_PUBLISH_FILES_PLUS_INDEX_EXCEEDS_ENTRIES_VAR_1} now and the rest in another publish to the same url
