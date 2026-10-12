<!--
name: 'Artifact: Stamp approve event under unrelated key'
description: >-
  Stamp approve event under unrelated key. Text emitted in an Artifact tool
  result or tool validation error.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_STAMP_INPUT_CARRIES_APPROVE_VERB_UNDER_VAR_0
-->
stamp.input.${TOOL_RESULT_ARTIFACT_STAMP_INPUT_CARRIES_APPROVE_VERB_UNDER_VAR_0} carries the approve verb under a non-event key — it must ride an event-named key or the write creates a pending draft
