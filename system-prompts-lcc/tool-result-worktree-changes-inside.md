<!--
name: 'Tool Result: worktree submodule — changes inside … ……'
description: ExitWorktree validation reports modified submodule paths.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_WORKTREE_CHANGES_INSIDE_VAR_0
  - TOOL_RESULT_WORKTREE_CHANGES_INSIDE_VAR_1
  - TOOL_RESULT_WORKTREE_CHANGES_INSIDE_VAR_2
-->
changes inside ${TOOL_RESULT_WORKTREE_CHANGES_INSIDE_VAR_0.paths.length===1?"submodule":"submodules"} ${TOOL_RESULT_WORKTREE_CHANGES_INSIDE_VAR_1.join(", ")}${TOOL_RESULT_WORKTREE_CHANGES_INSIDE_VAR_2>0?` and ${TOOL_RESULT_WORKTREE_CHANGES_INSIDE_VAR_2} more`:""}
