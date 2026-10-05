<!--
name: 'Permission ask: served MCP tool with unvouched path'
description: >-
  Ask-permission message explaining that Claude Code asks before one of its own
  served MCP tools runs with a path it cannot vouch for, telling the approver to
  check it does not reach this machine's Claude credentials.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_PERMISSION_ASK_SERVED_MCP_UNTRUSTED_PATH_VAR_0
-->
${TOOL_RESULT_PERMISSION_ASK_SERVED_MCP_UNTRUSTED_PATH_VAR_0} asks before one of its own MCP tools runs with a path it cannot vouch for from here (a relative path, a pattern, a variable, an encoded or quoted spelling, or a directory above its Claude credentials) — check it does not reach this machine's Claude credentials before approving.
