<!--
name: 'Tool result: WebSearch budget exhausted'
description: >-
  WebSearch tool result when the turn or session web search budget is used up,
  telling the model not to work around the limit.
ccVersion: 2.1.308
variables:
  - TOOL_RESULT_WEBSEARCH_SESSION_BUDGET_EXHAUSTED_VAR_0
  - TOOL_RESULT_WEBSEARCH_SESSION_BUDGET_EXHAUSTED_VAR_1
  - TOOL_RESULT_WEBSEARCH_SESSION_BUDGET_EXHAUSTED_VAR_2
  - TOOL_RESULT_WEBSEARCH_SESSION_BUDGET_EXHAUSTED_VAR_3
  - TOOL_RESULT_WEBSEARCH_SESSION_BUDGET_EXHAUSTED_VAR_4
-->
Web search was not performed: this ${TOOL_RESULT_WEBSEARCH_SESSION_BUDGET_EXHAUSTED_VAR_0}'s web search budget is used up (${TOOL_RESULT_WEBSEARCH_SESSION_BUDGET_EXHAUSTED_VAR_1}). ${TOOL_RESULT_WEBSEARCH_SESSION_BUDGET_EXHAUSTED_VAR_2}; do not work around the limit by querying search engines with curl or wget from ${TOOL_RESULT_WEBSEARCH_SESSION_BUDGET_EXHAUSTED_VAR_3}, by querying them in a browser or through a computer-use tool, or by searching or fetching through a third-party reader, proxy or archive service.${TOOL_RESULT_WEBSEARCH_SESSION_BUDGET_EXHAUSTED_VAR_4}
