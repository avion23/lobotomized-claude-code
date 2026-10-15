<!--
name: 'Tool Result: cloud session remote unreadable'
description: >-
  Notice that no remote could be read so the branch or HEAD could not be checked
  on the host
ccVersion: 2.1.301
variables:
  - TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_0
  - TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_1
  - TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_2
  - TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_3
  - TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_4
-->
${TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_0?`This checkout is on a detached HEAD, and no remote of it could be read, so its commit could not be looked for on ${TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_1}. The cloud session was asked to start from HEAD as ${TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_1} has it, its default branch.`:`Whether branch ${TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_2(TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_3)} is on ${TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_1} could not be checked, because no remote of this checkout could be read. The cloud session was asked to start from it by name.`}${TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_4.advisesPush?` ${TOOL_RESULT_CLOUD_SESSION_REMOTE_UNREADABLE_START_HINT_VAR_0?"To start from your work, push it":"If it is not there, push your work"} to a branch and start a new session from that branch.`:""}
