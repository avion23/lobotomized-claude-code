<!--
name: 'WebFetch: recent failure not refetched'
description: Not fetched because the URL failed seconds ago; carry on without it.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_WEBFETCH_RECENT_FAILURE_NOT_REFETCHED_VAR_0
  - TOOL_RESULT_WEBFETCH_RECENT_FAILURE_NOT_REFETCHED_VAR_1
  - TOOL_RESULT_WEBFETCH_RECENT_FAILURE_NOT_REFETCHED_VAR_2
  - TOOL_RESULT_WEBFETCH_RECENT_FAILURE_NOT_REFETCHED_VAR_3
-->
Not fetched: ${TOOL_RESULT_WEBFETCH_RECENT_FAILURE_NOT_REFETCHED_VAR_0} failed ${TOOL_RESULT_WEBFETCH_RECENT_FAILURE_NOT_REFETCHED_VAR_1}s ago in this session (${TOOL_RESULT_WEBFETCH_RECENT_FAILURE_NOT_REFETCHED_VAR_2.errorType}), and a second fetch this soon nearly always fails the same way. Carry on without this page and say that it could not be read. If another try was asked for in so many words, call ${TOOL_RESULT_WEBFETCH_RECENT_FAILURE_NOT_REFETCHED_VAR_3} again with the same url.
