<!--
name: Worktree git set variable readable
description: Fix to set a git-redirecting variable where the guard can read it
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_WORKTREE_GIT_SET_VAR_READABLE_VAR_0
  - TOOL_RESULT_BASH_WORKTREE_GIT_SET_VAR_READABLE_VAR_1
-->
Set ${TOOL_RESULT_BASH_WORKTREE_GIT_SET_VAR_READABLE_VAR_0} where this guard can read its value, on the command that needs it (${TOOL_RESULT_BASH_WORKTREE_GIT_SET_VAR_READABLE_VAR_0}=<value> <command>) or in an export (export ${TOOL_RESULT_BASH_WORKTREE_GIT_SET_VAR_READABLE_VAR_0}=<value>), and run it from ${TOOL_RESULT_BASH_WORKTREE_GIT_SET_VAR_READABLE_VAR_1}.
