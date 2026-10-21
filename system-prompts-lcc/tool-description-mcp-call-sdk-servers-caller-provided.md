<!--
name: 'Tool Description: mcp_call SDK servers caller-provided'
description: >-
  Middle fragment of the mcp_call description: SDK servers are rejected as
  caller-provided, result processing, session expiry and URL elicitation
  behaviour
ccVersion: 2.1.301
-->
they are caller-provided, so the caller can invoke them directly without the subprocess round-trip. Result content passes through the same processing as model-turn MCP calls, unless result_not_for_model is set. Session expiry is not retried automatically; callers can mcp_reconnect and retry. UrlElicitationRequired (-32042) tries Elicitation hooks; if no hook 
