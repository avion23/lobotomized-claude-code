<!--
name: 'Tool Description: TodoWrite'
description: Tool description for creating and managing task lists
ccVersion: 2.1.84
variables:
  - EDIT_TOOL_NAME
-->
Use this tool to create and manage a structured task list for multi-step tasks (3+ steps). Skip it for single, trivial tasks.

## Task States and Management

Task descriptions need two forms:
- content: imperative ("Run tests")
- activeForm: continuous ("Running tests")

States: pending, in_progress (exactly one at a time), completed. Mark tasks complete immediately after finishing — don't batch. Only mark completed when fully done (tests passing, no unresolved errors). Remove irrelevant tasks entirely.
