<!--
name: 'Tool Result: Artifact edits write-back skipped'
description: >-
  After publish, explains why the local file was left unchanged and asks to
  apply the same edits with Edit before republishing
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_SKIPPED_VAR_0
  - TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_SKIPPED_VAR_1
  - TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_SKIPPED_VAR_2
-->
${TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_SKIPPED_VAR_0} (${TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_SKIPPED_VAR_1==="changed_during_publish"?"it changed on disk while the publish ran, so it was left as it is":TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_SKIPPED_VAR_1==="not_writable"?"it could not be opened for writing (read-only), so it was left as it is":"it has other names on disk (a hard link), so it was left as it is"}). Apply the same ${TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_SKIPPED_VAR_2?"edit":"edits"} to that file with Edit before you publish it again${TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_SKIPPED_VAR_1==="hard_linked"?", and publish it without `edits` while it has other names":""}; publishing it as it is would revert ${TOOL_RESULT_ARTIFACT_EDITS_WRITEBACK_SKIPPED_VAR_2?"it":"them"}.
