<!--
name: 'Artifact read: input looks like a bare artifact id'
description: >-
  Guidance returned by the Artifact read handler when the given value looks like
  an artifact id/slug on its own rather than a full URL, telling the model to
  pass the full link.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_READ_LOOKS_LIKE_ARTIFACT_ID_PASS_FULL_LINK_VAR_0
  - TOOL_RESULT_ARTIFACT_READ_LOOKS_LIKE_ARTIFACT_ID_PASS_FULL_LINK_VAR_1
  - TOOL_RESULT_ARTIFACT_READ_LOOKS_LIKE_ARTIFACT_ID_PASS_FULL_LINK_VAR_2
  - TOOL_RESULT_ARTIFACT_READ_LOOKS_LIKE_ARTIFACT_ID_PASS_FULL_LINK_VAR_3
-->
${TOOL_RESULT_ARTIFACT_READ_LOOKS_LIKE_ARTIFACT_ID_PASS_FULL_LINK_VAR_0} that looks like an artifact id on its own; if it is one, pass the full link ${TOOL_RESULT_ARTIFACT_READ_LOOKS_LIKE_ARTIFACT_ID_PASS_FULL_LINK_VAR_1({slug:h,env:TOOL_RESULT_ARTIFACT_READ_LOOKS_LIKE_ARTIFACT_ID_PASS_FULL_LINK_VAR_2()})} as \`${TOOL_RESULT_ARTIFACT_READ_LOOKS_LIKE_ARTIFACT_ID_PASS_FULL_LINK_VAR_3.field??"url"}\`.
