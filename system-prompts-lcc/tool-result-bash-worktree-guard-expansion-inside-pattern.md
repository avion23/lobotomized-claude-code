<!--
name: Worktree guard expansion inside pattern
description: Guard reason and fix for an expansion inside a pattern
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_WORKTREE_GUARD_EXPANSION_INSIDE_PATTERN_VAR_0
  - TOOL_RESULT_BASH_WORKTREE_GUARD_EXPANSION_INSIDE_PATTERN_VAR_1
-->
an expansion inside the pattern ${TOOL_RESULT_BASH_WORKTREE_GUARD_EXPANSION_INSIDE_PATTERN_VAR_0(TOOL_RESULT_BASH_WORKTREE_GUARD_EXPANSION_INSIDE_PATTERN_VAR_1.text)} (a bare $NAME, \${NAME} or $1 passes; quote it, as "$NAME", when a [ or : follows; spell a literal $ as an unquoted \\$; put anything else, such as a nested \${…}, a backquote or a $'…' string, in a variable first)
