<!--
name: 'Tool Result: Bash worktree guard awk pipe operand'
description: >-
  Refusal reason for awk programs that pipe print or getline to a command, with
  a safe regex workaround
ccVersion: 2.1.299
-->
with a | after print/printf or before getline in its program, which awk can run as a pipe to a command, whatever the command is (a | in a regex, string or comment at such a spot is refused too: pass the pattern with -v re='a|b', doubling any backslash in it, and use $0 ~ re or gsub(re, "x"); print a literal | as "\\174")
