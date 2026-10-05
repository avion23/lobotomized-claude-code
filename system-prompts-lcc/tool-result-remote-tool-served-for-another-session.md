<!--
name: Remote tool call served for another session
description: >-
  Refusal for a call served for a different session than the one it's routed to
  run on.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_SERVED_FOR_ANOTHER_SESSION_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_SERVED_FOR_ANOTHER_SESSION_VAR_1
-->
${TOOL_RESULT_REMOTE_TOOL_SERVED_FOR_ANOTHER_SESSION_VAR_0.name} was not run: this session runs it on ${TOOL_RESULT_REMOTE_TOOL_SERVED_FOR_ANOTHER_SESSION_VAR_1.name}, and a call served for another session does not travel there.
