<!--
name: 'Tool Result: WebFetch proxy deadline'
description: >-
  Error when the WebFetch/WebSearch proxy did not finish before the deadline,
  noting it does not mean the page or query was bad
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_WEBFETCH_PROXY_DEADLINE_VAR_0
  - TOOL_RESULT_WEBFETCH_PROXY_DEADLINE_VAR_1
-->
The ${TOOL_RESULT_WEBFETCH_PROXY_DEADLINE_VAR_0} proxy had not finished answering after ${TOOL_RESULT_WEBFETCH_PROXY_DEADLINE_VAR_1/1000}s, so Claude Code stopped the request. This does not mean the ${TOOL_RESULT_WEBFETCH_PROXY_DEADLINE_VAR_0==="WebFetch"?"page is unavailable":"query was wrong"}. Trying again may work, but could take another ${TOOL_RESULT_WEBFETCH_PROXY_DEADLINE_VAR_1/1000}s.
