<!--
name: 'Tool Result: Cloud session branch not on remote'
description: >-
  Bundle-failure clause that the branch shares no history with the remote,
  optionally advising to push it
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_CLOUD_SESSION_BRANCH_NOT_ON_REMOTE_VAR_0
-->
. This branch shares no history with the remote as last fetched here${TOOL_RESULT_CLOUD_SESSION_BRANCH_NOT_ON_REMOTE_VAR_0?"; push it to start from GitHub instead":""}
