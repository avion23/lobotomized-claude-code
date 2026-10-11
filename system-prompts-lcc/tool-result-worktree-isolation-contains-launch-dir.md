<!--
name: 'Tool Result: Isolation worktree contains the launch directory'
description: >-
  EnterWorktree/Agent isolation error when the worktree contains the directory
  this run started from and nothing vouches for its worktree registration.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_WORKTREE_ISOLATION_CONTAINS_LAUNCH_DIR_VAR_0
-->
The worktree ${TOOL_RESULT_WORKTREE_ISOLATION_CONTAINS_LAUNCH_DIR_VAR_0} contains the directory this resume ran from, and nothing in this session vouches for its worktree registration — an isolation worktree never contains its own launch position. Run the resume from the project checkout instead.
