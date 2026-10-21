<!--
name: 'Tool result: EnterWorktree locked by other session'
description: >-
  EnterWorktree error when the worktree belongs to another running Claude Code
  session.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_ENTERWORKTREE_LOCKED_BY_OTHER_SESSION_VAR_0
  - TOOL_RESULT_ENTERWORKTREE_LOCKED_BY_OTHER_SESSION_VAR_1
  - TOOL_RESULT_ENTERWORKTREE_LOCKED_BY_OTHER_SESSION_VAR_2
-->
Cannot enter worktree: ${TOOL_RESULT_ENTERWORKTREE_LOCKED_BY_OTHER_SESSION_VAR_0} belongs to another running Claude Code session (locked: ${TOOL_RESULT_ENTERWORKTREE_LOCKED_BY_OTHER_SESSION_VAR_1(TOOL_RESULT_ENTERWORKTREE_LOCKED_BY_OTHER_SESSION_VAR_2.lockReason??"")}). Wait for that session to finish or choose a different worktree.
