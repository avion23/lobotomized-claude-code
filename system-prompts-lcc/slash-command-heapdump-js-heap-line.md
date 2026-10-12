<!--
name: 'Slash Command: /heapdump JS heap line'
description: Bun-runtime /heapdump diagnostics line giving JS heap size (in snapshot).
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_HEAPDUMP_JS_HEAP_LINE_VAR_0
  - SLASH_COMMAND_HEAPDUMP_JS_HEAP_LINE_VAR_1
-->
  JS heap          ${SLASH_COMMAND_HEAPDUMP_JS_HEAP_LINE_VAR_0(SLASH_COMMAND_HEAPDUMP_JS_HEAP_LINE_VAR_1.heapUsed).padStart(8)}  in snapshot
