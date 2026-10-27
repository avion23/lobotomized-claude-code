<!--
name: Worktree git search without find -exec
description: Fix to search without find -exec or spell git options literally
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_WORKTREE_GIT_FIND_EXEC_SEARCH_WITHOUT_VAR_0
-->
If git is only a search pattern there, search without find -exec (grep -rl git .); otherwise spell git's options and subcommand out literally and run it from ${TOOL_RESULT_BASH_WORKTREE_GIT_FIND_EXEC_SEARCH_WITHOUT_VAR_0}.
