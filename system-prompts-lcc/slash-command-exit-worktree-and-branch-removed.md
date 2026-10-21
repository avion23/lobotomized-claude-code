<!--
name: 'Slash command: exit worktree and branch removed'
description: >-
  Exit-worktree result when commit count is unknown for a git worktree: worktree
  and its branch removed, with optional discarded-changes and tmux notes.
ccVersion: 2.1.301
variables:
  - SLASH_COMMAND_EXIT_WORKTREE_AND_BRANCH_REMOVED_VAR_0
  - SLASH_COMMAND_EXIT_WORKTREE_AND_BRANCH_REMOVED_VAR_1
  - SLASH_COMMAND_EXIT_WORKTREE_AND_BRANCH_REMOVED_VAR_2
  - SLASH_COMMAND_EXIT_WORKTREE_AND_BRANCH_REMOVED_VAR_3
-->
Worktree and branch ${SLASH_COMMAND_EXIT_WORKTREE_AND_BRANCH_REMOVED_VAR_0.worktreeBranch} removed.${SLASH_COMMAND_EXIT_WORKTREE_AND_BRANCH_REMOVED_VAR_1>0?` Uncommitted changes were ${SLASH_COMMAND_EXIT_WORKTREE_AND_BRANCH_REMOVED_VAR_2}`:""}${SLASH_COMMAND_EXIT_WORKTREE_AND_BRANCH_REMOVED_VAR_3}
