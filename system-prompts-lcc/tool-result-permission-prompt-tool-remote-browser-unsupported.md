<!--
name: 'Tool Result: Permission prompt tool on remote-browser not allowed'
description: >-
  Deny message saying a call was not run because the configured permission
  prompt tool belongs to the remote-browser MCP server, which can't answer
  permission requests
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_PERMISSION_PROMPT_TOOL_REMOTE_BROWSER_UNSUPPORTED_VAR_0
  - TOOL_RESULT_PERMISSION_PROMPT_TOOL_REMOTE_BROWSER_UNSUPPORTED_VAR_1
-->
${TOOL_RESULT_PERMISSION_PROMPT_TOOL_REMOTE_BROWSER_UNSUPPORTED_VAR_0.name} was not run. The permission prompt tool ${TOOL_RESULT_PERMISSION_PROMPT_TOOL_REMOTE_BROWSER_UNSUPPORTED_VAR_1} is a tool of MCP server 'remote-browser', and in this session that server's tools can't answer permission requests, because nothing would check the call to it. To have these requests answered, set --permission-prompt-tool to a tool of another MCP server.
