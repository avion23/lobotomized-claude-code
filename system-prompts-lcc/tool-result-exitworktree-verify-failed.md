<!--
name: 'Tool result: ExitWorktree verify failed'
description: >-
  ExitWorktree validation error when worktree state cannot be verified,
  requiring discard_changes or keep.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_EXITWORKTREE_VERIFY_FAILED_VAR_0
  - TOOL_RESULT_EXITWORKTREE_VERIFY_FAILED_VAR_1
-->
Could not verify worktree state at ${TOOL_RESULT_EXITWORKTREE_VERIFY_FAILED_VAR_0(TOOL_RESULT_EXITWORKTREE_VERIFY_FAILED_VAR_1.worktreePath)}. Refusing to remove without explicit confirmation. Re-invoke with discard_changes: true to proceed — or use action: "keep" to preserve the worktree.
