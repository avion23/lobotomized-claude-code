<!--
name: 'Tool Result: ExitWorktree verify failed'
description: >-
  Refusal to remove a worktree whose state could not be verified without
  explicit confirmation
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_EXITWORKTREE_VERIFY_FAILED_VAR_0
  - TOOL_RESULT_EXITWORKTREE_VERIFY_FAILED_VAR_1
  - TOOL_RESULT_EXITWORKTREE_VERIFY_FAILED_VAR_2
-->
Could not verify worktree state at ${TOOL_RESULT_EXITWORKTREE_VERIFY_FAILED_VAR_0(TOOL_RESULT_EXITWORKTREE_VERIFY_FAILED_VAR_1.worktreePath)}.${TOOL_RESULT_EXITWORKTREE_VERIFY_FAILED_VAR_2} Refusing to remove without explicit confirmation. Confirm with the user, then re-invoke with discard_changes: true to proceed — or use action: "keep" to preserve the worktree.
