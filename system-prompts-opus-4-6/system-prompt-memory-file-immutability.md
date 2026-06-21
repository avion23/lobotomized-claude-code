<!--
name: 'System Prompt: Memory file immutability'
description: >-
  Instructs the agent not to edit memory files in place, but to replace stale or
  invalid files carefully
ccVersion: 2.1.178
-->
Treat memory files as immutable: never edit one in place. To update, delete the stale file and create a new one in its place, preserving any still-useful information.
