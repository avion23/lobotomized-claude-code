<!--
name: ExitWorktree unmerged-commit warning
description: >-
  Commit-count and branch detail included in the refusal to remove a worktree
  without discard confirmation.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_EXITWORKTREE_UNMERGED_COMMIT_COUNT_VAR_0
  - TOOL_RESULT_EXITWORKTREE_UNMERGED_COMMIT_COUNT_VAR_1
-->
${TOOL_RESULT_EXITWORKTREE_UNMERGED_COMMIT_COUNT_VAR_0} ${TOOL_RESULT_EXITWORKTREE_UNMERGED_COMMIT_COUNT_VAR_0===1?"commit":"commits"} on ${TOOL_RESULT_EXITWORKTREE_UNMERGED_COMMIT_COUNT_VAR_1.worktreeBranch??"the worktree branch"}
