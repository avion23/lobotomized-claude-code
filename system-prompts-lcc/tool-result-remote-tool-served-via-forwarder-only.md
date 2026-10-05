<!--
name: Remote tool requires forwarder
description: >-
  Refuses a direct call to a tool that is only served for remote tool execution
  and must go through a cloud session's forwarder.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_SERVED_VIA_FORWARDER_ONLY_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_SERVED_VIA_FORWARDER_ONLY_VAR_1
-->
${TOOL_RESULT_REMOTE_TOOL_SERVED_VIA_FORWARDER_ONLY_VAR_0} on ${TOOL_RESULT_REMOTE_TOOL_SERVED_VIA_FORWARDER_ONLY_VAR_1} is served for Claude Code remote tool execution and must be called through a cloud session's forwarder.
