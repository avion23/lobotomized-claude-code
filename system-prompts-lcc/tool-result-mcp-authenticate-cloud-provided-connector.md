<!--
name: MCP authenticate cloud-provided connector
description: >-
  Message that a connector is provided by the cloud service and cannot be signed
  in from here
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_MCP_AUTHENTICATE_CLOUD_PROVIDED_CONNECTOR_VAR_0
  - TOOL_RESULT_MCP_AUTHENTICATE_CLOUD_PROVIDED_CONNECTOR_VAR_1
-->
"${TOOL_RESULT_MCP_AUTHENTICATE_CLOUD_PROVIDED_CONNECTOR_VAR_0(TOOL_RESULT_MCP_AUTHENTICATE_CLOUD_PROVIDED_CONNECTOR_VAR_1)}" is provided to this session by Claude Code's cloud service, which holds its sign-in, so it can't be signed in to from here. If it is one of your claude.ai connectors, reconnect it under Settings → Connectors on claude.ai and then start a new session.
