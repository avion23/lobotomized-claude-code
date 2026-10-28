<!--
name: Worktree git find -exec braces
description: 'Refusal that {} after git is filled by find -exec'
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_WORKTREE_GIT_FIND_EXEC_BRACES_VAR_0
  - TOOL_RESULT_BASH_WORKTREE_GIT_FIND_EXEC_BRACES_VAR_1
-->
has {} among the words right after git (${TOOL_RESULT_BASH_WORKTREE_GIT_FIND_EXEC_BRACES_VAR_0(TOOL_RESULT_BASH_WORKTREE_GIT_FIND_EXEC_BRACES_VAR_1.runtime)}), which find -exec fills with a path name when the command runs, so the options git receives can't be verified
