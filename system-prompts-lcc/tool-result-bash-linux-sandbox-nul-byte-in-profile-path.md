<!--
name: 'Tool Result: Linux Sandbox NUL Byte In Profile Path'
description: >-
  Error surfaced when a path in the Linux sandbox profile contains a NUL byte,
  which bwrap's argument list or args-file cannot carry, blocking the sandboxed
  Bash command.
ccVersion: 2.1.284
-->
Sandbox profile contains a path with a NUL byte, which neither a command line nor a file of bwrap arguments can carry
