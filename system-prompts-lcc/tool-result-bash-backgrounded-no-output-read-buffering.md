<!--
name: 'Tool Result: Bash backgrounded with no output read'
description: >-
  Note that no output had been read when moved and buffering programs may keep
  the output file empty
ccVersion: 2.1.311
-->
No output had been read from it when it was moved. A program that buffers its output, or a pipe into one such as tail, can keep the output file empty until the command finishes.
