<!--
name: 'Tool Result: cloud session branch ahead of remote'
description: >-
  Notice that the branch is ahead of its remote so the cloud session starts
  without those commits
ccVersion: 2.1.301
variables:
  - TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_0
  - TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_1
  - TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_2
  - TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_3
  - TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_4
-->
Branch ${TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_0} is ${TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_1?"1 commit":`${TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_2.toLocaleString("en-US")} commits`} ahead of ${TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_3}/${TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_0} (as last fetched), so the cloud session starts without ${TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_1?"it":"them"} and without any uncommitted changes.${TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_4?` Push the branch and start a new session to have ${TOOL_RESULT_CLOUD_SESSION_BRANCH_AHEAD_OF_REMOTE_VAR_1?"that commit":"those commits"}.`:""}
