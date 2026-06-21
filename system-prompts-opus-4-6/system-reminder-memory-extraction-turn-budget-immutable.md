<!--
name: 'System Reminder: Memory extraction turn budget (immutable)'
description: >-
  Instructs the memory extraction subagent to batch memory writes and deletes
  when memory files are immutable
ccVersion: 2.1.178
variables:
  - WRITE_TOOL_NAME
  - MEMORY_DELETE_COMMAND
-->
Issue all ${WRITE_TOOL_NAME} and ${MEMORY_DELETE_COMMAND} calls in one turn — there is no read-then-edit step.
