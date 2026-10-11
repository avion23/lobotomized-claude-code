<!--
name: 'Tool Result: WorktreeCreate Hook Failed Errors'
description: 'Error when the WorktreeCreate hook fails, listing the hook errors.'
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_WORKTREE_CREATE_HOOK_FAILED_ERRORS_VAR_0
-->
WorktreeCreate hook failed: ${TOOL_RESULT_WORKTREE_CREATE_HOOK_FAILED_ERRORS_VAR_0.join("; ")}
