<!--
name: 'Tool Result: WebFetch permission retries fail'
description: >-
  Says retries will fail and, without a user to ask, to continue without the
  page and report the URL
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_WEBFETCH_PERMISSION_SUBAGENT_RETRIES_FAIL_VAR_0
  - TOOL_RESULT_WEBFETCH_PERMISSION_SUBAGENT_RETRIES_FAIL_VAR_1
  - TOOL_RESULT_WEBFETCH_PERMISSION_SUBAGENT_RETRIES_FAIL_VAR_2
-->
${TOOL_RESULT_WEBFETCH_PERMISSION_SUBAGENT_RETRIES_FAIL_VAR_0??TOOL_RESULT_WEBFETCH_PERMISSION_SUBAGENT_RETRIES_FAIL_VAR_1??TOOL_RESULT_WEBFETCH_PERMISSION_SUBAGENT_RETRIES_FAIL_VAR_2} Retries will fail. If you cannot ask the user (e.g. from a subagent), continue without this page and report the blocked URL in your findings.
