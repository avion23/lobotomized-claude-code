<!--
name: 'Tool Result: agent worktree hook path is not a directory'
description: >-
  Agent worktree isolation error when the WorktreeCreate hook echoed a path that
  is not a directory.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_AGENT_WORKTREE_HOOK_PATH_NOT_DIRECTORY_VAR_0
-->
WorktreeCreate hook returned a path that is not a directory: ${TOOL_RESULT_AGENT_WORKTREE_HOOK_PATH_NOT_DIRECTORY_VAR_0}. The hook must create the directory before echoing its path.
