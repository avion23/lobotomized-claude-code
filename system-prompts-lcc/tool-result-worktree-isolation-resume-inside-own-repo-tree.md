<!--
name: 'Tool Result: Worktree resume started inside its own repository tree'
description: >-
  EnterWorktree/Agent isolation error when the launch directory is inside the
  worktree, which is its own repository, so it cannot be confirmed as a separate
  isolation worktree.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_WORKTREE_ISOLATION_RESUME_INSIDE_OWN_REPO_TREE_VAR_0
-->
This resume was started from inside ${TOOL_RESULT_WORKTREE_ISOLATION_RESUME_INSIDE_OWN_REPO_TREE_VAR_0} (or a directory it contains), which is its own repository — it cannot be confirmed as a separate isolation worktree from there. Run the resume from the project checkout instead.
