<!--
name: >-
  Tool Result: WebFetch — proxy rate limited, wait the requested time before
  retrying
description: >-
  Tells the model the proxy was rate limited and how many seconds the server
  asks it to wait before retrying.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_WEBFETCH_PROXY_RATE_LIMITED_RETRY_AFTER_VAR_0
  - TOOL_RESULT_WEBFETCH_PROXY_RATE_LIMITED_RETRY_AFTER_VAR_1
-->
; rate limited — the server requests waiting ~${TOOL_RESULT_WEBFETCH_PROXY_RATE_LIMITED_RETRY_AFTER_VAR_0.ceil(TOOL_RESULT_WEBFETCH_PROXY_RATE_LIMITED_RETRY_AFTER_VAR_1/1000)}s before retrying
