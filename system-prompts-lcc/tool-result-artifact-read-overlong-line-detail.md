<!--
name: Overlong-line number/char-count detail
description: >-
  The per-line 'line N (M characters...)' detail template S=(a)=>... used to
  list individual overlong lines in the artifact-read tool result.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_READ_OVERLONG_LINE_DETAIL_VAR_0
  - TOOL_RESULT_ARTIFACT_READ_OVERLONG_LINE_DETAIL_VAR_1
-->
line ${TOOL_RESULT_ARTIFACT_READ_OVERLONG_LINE_DETAIL_VAR_0(TOOL_RESULT_ARTIFACT_READ_OVERLONG_LINE_DETAIL_VAR_1.line)} (${TOOL_RESULT_ARTIFACT_READ_OVERLONG_LINE_DETAIL_VAR_0(TOOL_RESULT_ARTIFACT_READ_OVERLONG_LINE_DETAIL_VAR_1.chars)} characters${TOOL_RESULT_ARTIFACT_READ_OVERLONG_LINE_DETAIL_VAR_1.verdict==="differs"?", which differs from the content you sent":TOOL_RESULT_ARTIFACT_READ_OVERLONG_LINE_DETAIL_VAR_1.verdict==="same"?", identical to a line you sent":""})
