<!--
name: Ordered query returns one page note (Artifact DB)
description: >-
  Note included in a db_read tool_result explaining that ordered queries return
  only the first page, embedding the Z suggestion.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_DB_ORDERED_QUERY_ONE_PAGE_NOTE_VAR_0
  - TOOL_RESULT_ARTIFACT_DB_ORDERED_QUERY_ONE_PAGE_NOTE_VAR_1
  - TOOL_RESULT_ARTIFACT_DB_ORDERED_QUERY_ONE_PAGE_NOTE_VAR_2
  - TOOL_RESULT_ARTIFACT_DB_ORDERED_QUERY_ONE_PAGE_NOTE_VAR_3
-->

[ordered queries return one page: these are the first ${TOOL_RESULT_ARTIFACT_DB_ORDERED_QUERY_ONE_PAGE_NOTE_VAR_0.length} by ${TOOL_RESULT_ARTIFACT_DB_ORDERED_QUERY_ONE_PAGE_NOTE_VAR_1(TOOL_RESULT_ARTIFACT_DB_ORDERED_QUERY_ONE_PAGE_NOTE_VAR_2.ordered_by.field)} — more may exist. ${TOOL_RESULT_ARTIFACT_DB_ORDERED_QUERY_ONE_PAGE_NOTE_VAR_3}]
