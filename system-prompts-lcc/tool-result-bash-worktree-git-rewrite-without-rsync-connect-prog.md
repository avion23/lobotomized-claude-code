<!--
name: Worktree git rewrite without RSYNC_CONNECT_PROG
description: Fix to rewrite the command without RSYNC_CONNECT_PROG
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_WORKTREE_GIT_REWRITE_WITHOUT_RSYNC_CONNECT_PROG_VAR_0
-->
Rewrite the command so that it does not spell RSYNC_CONNECT_PROG and run it from ${TOOL_RESULT_BASH_WORKTREE_GIT_REWRITE_WITHOUT_RSYNC_CONNECT_PROG_VAR_0}; a transfer that needs that connection program belongs to a session that is not isolated to a worktree.
