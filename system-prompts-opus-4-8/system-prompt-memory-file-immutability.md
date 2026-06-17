<!--
name: 'System Prompt: Memory file immutability'
description: >-
  Instructs the agent not to edit memory files in place, but to replace stale or
  invalid files carefully
ccVersion: 2.1.178
-->
Treat memory files as immutable; don't edit a memory file in-place to update it. Instead, delete memory files that have become stale or invalid and create new ones in their place, taking care that no useful information is lost in the switch.
