<!--
name: 'Tool result: EnterWorktree cwd is the repository root'
description: >-
  EnterWorktree refusal in a pinned-cwd session when the current working
  directory is the repository root rather than a worktree.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ENTERWORKTREE_CWD_IS_REPOSITORY_ROOT_VAR_0
-->
Cannot enter worktree: the current working directory ${TOOL_RESULT_ENTERWORKTREE_CWD_IS_REPOSITORY_ROOT_VAR_0} is the repository root, not an isolated worktree — switching is only available to sessions whose working directory is inside a worktree of this repository.
