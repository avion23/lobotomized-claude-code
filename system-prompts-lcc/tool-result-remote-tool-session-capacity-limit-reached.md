<!--
name: Remote-tool session capacity reached
description: >-
  Tells the model the target machine already holds the maximum number of cloud
  sessions' state and this session wasn't added, so it should not retry in a
  loop.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_SESSION_CAPACITY_LIMIT_REACHED_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_SESSION_CAPACITY_LIMIT_REACHED_VAR_1
  - TOOL_RESULT_REMOTE_TOOL_SESSION_CAPACITY_LIMIT_REACHED_VAR_2
-->
${TOOL_RESULT_REMOTE_TOOL_SESSION_CAPACITY_LIMIT_REACHED_VAR_0} already keeps state for ${TOOL_RESULT_REMOTE_TOOL_SESSION_CAPACITY_LIMIT_REACHED_VAR_1} cloud ${TOOL_RESULT_REMOTE_TOOL_SESSION_CAPACITY_LIMIT_REACHED_VAR_2(TOOL_RESULT_REMOTE_TOOL_SESSION_CAPACITY_LIMIT_REACHED_VAR_1,"session")}, the most it holds at once — this session was not added and nothing ran. Tell the user: restarting Claude Code on ${TOOL_RESULT_REMOTE_TOOL_SESSION_CAPACITY_LIMIT_REACHED_VAR_0} frees those seats. Do not retry in a loop.
