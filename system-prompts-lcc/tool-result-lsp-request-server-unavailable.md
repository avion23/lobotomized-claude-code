<!--
name: 'Tool result: LSP request server unavailable'
description: >-
  LSP tool error detail when a request reaches a language server that is not
  running or not initialized (e.g. still starting); it is the message slot of
  the LSP tool's 'Error performing <operation>: …' result.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_LSP_REQUEST_SERVER_UNAVAILABLE_VAR_0
  - TOOL_RESULT_LSP_REQUEST_SERVER_UNAVAILABLE_VAR_1
  - TOOL_RESULT_LSP_REQUEST_SERVER_UNAVAILABLE_VAR_2
-->
Cannot send request to LSP server '${TOOL_RESULT_LSP_REQUEST_SERVER_UNAVAILABLE_VAR_0}': server is ${TOOL_RESULT_LSP_REQUEST_SERVER_UNAVAILABLE_VAR_1}${TOOL_RESULT_LSP_REQUEST_SERVER_UNAVAILABLE_VAR_2?`, last error: ${TOOL_RESULT_LSP_REQUEST_SERVER_UNAVAILABLE_VAR_2.message}`:""}
