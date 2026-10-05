<!--
name: 'Tool Result: Artifact workshop source not handed over'
description: >-
  Artifact tool result explaining that a workshop page's source is withheld and
  the model must read its live decisions via read_page_data instead of resending
  unchanged prior content
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_WORKSHOP_SOURCE_NOT_HANDED_OVER_VAR_0
  - TOOL_RESULT_ARTIFACT_WORKSHOP_SOURCE_NOT_HANDED_OVER_VAR_1
-->
It is a workshop page, so its source is not handed over: read its live decisions with the ${TOOL_RESULT_ARTIFACT_WORKSHOP_SOURCE_NOT_HANDED_OVER_VAR_0} tool's read_page_data action (schema "workshop-decisions") — that normally counts as viewing this version — then ${TOOL_RESULT_ARTIFACT_WORKSHOP_SOURCE_NOT_HANDED_OVER_VAR_1} — do not resend your previous content unchanged. The workshop skill forbids a content read and force here.
