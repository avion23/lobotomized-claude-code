<!--
name: 'Slash Command: Exit worktree removed, branch kept'
description: >-
  Exit-worktree result that the worktree was removed and the branch it was on is
  kept
ccVersion: 2.1.304
variables:
  - SLASH_COMMAND_EXIT_WORKTREE_REMOVED_BRANCH_KEPT_VAR_0
  - SLASH_COMMAND_EXIT_WORKTREE_REMOVED_BRANCH_KEPT_VAR_1
-->
Worktree removed. ${SLASH_COMMAND_EXIT_WORKTREE_REMOVED_BRANCH_KEPT_VAR_0(SLASH_COMMAND_EXIT_WORKTREE_REMOVED_BRANCH_KEPT_VAR_1.branch)?"The branch that it was on":`Branch ${SLASH_COMMAND_EXIT_WORKTREE_REMOVED_BRANCH_KEPT_VAR_1.branch}`} is kept.
