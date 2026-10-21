<!--
name: 'Tool result: ExitWorktree not owner'
description: >-
  ExitWorktree validation error refusing to remove a worktree this session does
  not own.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_EXITWORKTREE_NOT_OWNER_VAR_0
  - TOOL_RESULT_EXITWORKTREE_NOT_OWNER_VAR_1
-->
This session is not the owner of the worktree at ${TOOL_RESULT_EXITWORKTREE_NOT_OWNER_VAR_0(TOOL_RESULT_EXITWORKTREE_NOT_OWNER_VAR_1.worktreePath)} — it either entered a pre-existing worktree via EnterWorktree({path}) or resumed into a checkout whose liveness lock another running Claude Code session still holds — so this tool will not remove it. Use action: "keep" to return to ${TOOL_RESULT_EXITWORKTREE_NOT_OWNER_VAR_0(TOOL_RESULT_EXITWORKTREE_NOT_OWNER_VAR_1.originalCwd)}. If no other session is using it, remove it yourself with \`git worktree remove\`; while a live session's lock is present, git will refuse and name the owner.
