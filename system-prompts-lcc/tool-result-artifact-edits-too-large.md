<!--
name: 'Tool Result: Artifact edits too large'
description: >-
  Rejects Artifact edits whose old_str and new_str exceed the size cap and
  points to Edit plus a plain publish
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_ARTIFACT_EDITS_TOO_LARGE_VAR_0
-->
old_str and new_str add up to more than ${TOOL_RESULT_ARTIFACT_EDITS_TOO_LARGE_VAR_0} characters over all the edits; make a change that large with Edit and publish without edits
