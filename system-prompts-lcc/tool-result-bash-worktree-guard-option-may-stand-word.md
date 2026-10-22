<!--
name: 'Tool Result: worktree guard word may be read as option'
description: >-
  Longer reason that an unquoted/computed word may begin with - and be read as
  an option even after --, with remedies.
ccVersion: 2.1.308
-->
where an option may stand (a word that is not double-quoted, or whose first character is matched or computed rather than spelled out, may begin with - and be read as an option, even after --; spell it out, running any command substitution as its own command first, or, where the command is otherwise plain, begin a relative path or glob with ./ (a home path with ~/), quote an unquoted variable or a pattern meant for the program, or give an option its value as a separate word)
