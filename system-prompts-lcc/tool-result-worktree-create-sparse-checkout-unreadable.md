<!--
name: Worktree sparse checkout unreadable files
description: >-
  Error that a sparse worktree checkout left out unreadable files so it was
  removed
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_WORKTREE_CREATE_SPARSE_CHECKOUT_UNREADABLE_VAR_0
  - TOOL_RESULT_WORKTREE_CREATE_SPARSE_CHECKOUT_UNREADABLE_VAR_1
-->
Failed to checkout sparse worktree: git left out files whose contents it could not read, so the new worktree was removed.${TOOL_RESULT_WORKTREE_CREATE_SPARSE_CHECKOUT_UNREADABLE_VAR_0(TOOL_RESULT_WORKTREE_CREATE_SPARSE_CHECKOUT_UNREADABLE_VAR_1)}
