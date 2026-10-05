<!--
name: Artifact HTML byte/line-length summary clause
description: >-
  The 'N bytes, N lines, each/every line short enough to Read with offset/limit'
  clause inside Wkt({html,ver,...}), embedded parenthetically in the
  model-facing 'raw HTML saved to ...' tool result (see
  tool-result-artifact-read-summary-html-saved).
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_READ_HTML_LINE_LENGTH_SUMMARY_VAR_0
  - TOOL_RESULT_ARTIFACT_READ_HTML_LINE_LENGTH_SUMMARY_VAR_1
-->
${TOOL_RESULT_ARTIFACT_READ_HTML_LINE_LENGTH_SUMMARY_VAR_0}, ${TOOL_RESULT_ARTIFACT_READ_HTML_LINE_LENGTH_SUMMARY_VAR_1?"each":"every line"} short enough to Read with offset/limit
