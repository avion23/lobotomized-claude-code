<!--
name: 'Slash command: exit worktree removed (hook-based)'
description: >-
  Exit-worktree result for a WorktreeCreate-hook worktree whose commit count is
  unknown: worktree removed, with optional discarded-changes and tmux notes.
ccVersion: 2.1.301
variables:
  - SLASH_COMMAND_EXIT_WORKTREE_REMOVED_HOOK_BASED_VAR_0
  - SLASH_COMMAND_EXIT_WORKTREE_REMOVED_HOOK_BASED_VAR_1
  - SLASH_COMMAND_EXIT_WORKTREE_REMOVED_HOOK_BASED_VAR_2
-->
Worktree removed.${SLASH_COMMAND_EXIT_WORKTREE_REMOVED_HOOK_BASED_VAR_0>0?` Uncommitted changes were ${SLASH_COMMAND_EXIT_WORKTREE_REMOVED_HOOK_BASED_VAR_1}`:""}${SLASH_COMMAND_EXIT_WORKTREE_REMOVED_HOOK_BASED_VAR_2}
