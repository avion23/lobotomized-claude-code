<!--
name: 'Tool Result: Artifact edit old_str ambiguous'
description: >-
  Reports an Artifact edit whose old_str occurs more than once and asks for more
  surrounding text
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_ARTIFACT_EDITS_OLD_STR_AMBIGUOUS_VAR_0
  - TOOL_RESULT_ARTIFACT_EDITS_OLD_STR_AMBIGUOUS_VAR_1
-->
edits[${TOOL_RESULT_ARTIFACT_EDITS_OLD_STR_AMBIGUOUS_VAR_0.edit}] old_str occurs ${TOOL_RESULT_ARTIFACT_EDITS_OLD_STR_AMBIGUOUS_VAR_0.count>=TOOL_RESULT_ARTIFACT_EDITS_OLD_STR_AMBIGUOUS_VAR_1?"at least ":""}${TOOL_RESULT_ARTIFACT_EDITS_OLD_STR_AMBIGUOUS_VAR_0.count} times in the file; include more of the surrounding text so that it occurs once
