<!--
name: Suggest raising query.limit (Artifact DB)
description: >-
  Suggestion text appended to an ordered-query db_read tool_result when the
  limit is below the server cap.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_DB_QUERY_LIMIT_INCREASE_SUGGESTION_VAR_0
-->
Pass \`query.limit\` (up to ${TOOL_RESULT_ARTIFACT_DB_QUERY_LIMIT_INCREASE_SUGGESTION_VAR_0}) for a larger page, or drop \`query.order_by\` and page with \`query.cursor\` to read them all.
