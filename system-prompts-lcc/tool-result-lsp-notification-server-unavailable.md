<!--
name: 'Tool result: LSP notification server unavailable'
description: >-
  LSP error detail when a notification (didOpen) is sent to a language server
  that is not running or not initialized; wrapped as 'Failed to sync file open
  <file>: …' and returned in the LSP tool's 'Error performing <operation>: …'
  result.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_LSP_NOTIFICATION_SERVER_UNAVAILABLE_VAR_0
  - TOOL_RESULT_LSP_NOTIFICATION_SERVER_UNAVAILABLE_VAR_1
-->
Cannot send notification to LSP server '${TOOL_RESULT_LSP_NOTIFICATION_SERVER_UNAVAILABLE_VAR_0}': server is ${TOOL_RESULT_LSP_NOTIFICATION_SERVER_UNAVAILABLE_VAR_1}
