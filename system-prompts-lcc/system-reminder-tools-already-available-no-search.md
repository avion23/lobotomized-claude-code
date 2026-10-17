<!--
name: 'System reminder: tools already available, no search needed'
description: >-
  Meta message after a ToolSearch telling the model the requested tools are
  already loaded and can be called directly.
ccVersion: 2.1.302
variables:
  - SYSTEM_REMINDER_TOOLS_ALREADY_AVAILABLE_NO_SEARCH_VAR_0
-->
Already available in this conversation: ${SYSTEM_REMINDER_TOOLS_ALREADY_AVAILABLE_NO_SEARCH_VAR_0.join(", ")}. Call ${SYSTEM_REMINDER_TOOLS_ALREADY_AVAILABLE_NO_SEARCH_VAR_0.length===1?"it":"them"} directly; no search is needed.
