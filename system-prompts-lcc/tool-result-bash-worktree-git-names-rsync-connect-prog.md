<!--
name: Worktree git RSYNC_CONNECT_PROG
description: Refusal that the command names RSYNC_CONNECT_PROG
ccVersion: 2.1.310
-->
names RSYNC_CONNECT_PROG (in any letter case, possibly split by quotes, $ expansions, backticks, backslashes or brace lists), which is refused here even as a mere mention because rsync runs its value through the shell with the destination host spliced in, so what it runs cannot be shown not to be git
