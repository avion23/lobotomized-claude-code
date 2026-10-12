<!--
name: 'Tool Result: grep no — Found … total … across … ….…'
description: Grep count result reports pagination and aggregate occurrence totals.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_GREP_FOUND_TOTAL_ACROSS_VAR_0
  - TOOL_RESULT_GREP_FOUND_TOTAL_ACROSS_VAR_1
  - TOOL_RESULT_GREP_FOUND_TOTAL_ACROSS_VAR_2
-->


Found ${TOOL_RESULT_GREP_FOUND_TOTAL_ACROSS_VAR_0} total ${TOOL_RESULT_GREP_FOUND_TOTAL_ACROSS_VAR_0===1?"occurrence":"occurrences"} across ${TOOL_RESULT_GREP_FOUND_TOTAL_ACROSS_VAR_1} ${TOOL_RESULT_GREP_FOUND_TOTAL_ACROSS_VAR_1===1?"file":"files"}.${TOOL_RESULT_GREP_FOUND_TOTAL_ACROSS_VAR_2?` with pagination = ${TOOL_RESULT_GREP_FOUND_TOTAL_ACROSS_VAR_2}`:""}
