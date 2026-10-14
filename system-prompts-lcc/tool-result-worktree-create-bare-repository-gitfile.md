<!--
name: 'Tool Result: Worktree create from bare repository gitfile'
description: >-
  Refuses to create a worktree where .git points to a bare repository and
  suggests starting in one of its worktrees
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_WORKTREE_CREATE_BARE_REPOSITORY_GITFILE_VAR_0
  - TOOL_RESULT_WORKTREE_CREATE_BARE_REPOSITORY_GITFILE_VAR_1
-->
The .git in ${TOOL_RESULT_WORKTREE_CREATE_BARE_REPOSITORY_GITFILE_VAR_0(TOOL_RESULT_WORKTREE_CREATE_BARE_REPOSITORY_GITFILE_VAR_1)} points to a bare repository, so Claude Code can't create a worktree from this directory. Start Claude Code in one of that repository's worktrees instead (git worktree add makes one).
