<!--
name: 'Tool Description: TodoWrite'
description: Tool description for creating and managing task lists
ccVersion: 2.1.84
variables:
  - EDIT_TOOL_NAME
-->
Create and manage a task list for the current session. Tracks progress on multi-step work and shows the user where you are.

Use it when:
- Work has 3+ distinct steps the user is likely to want to follow
- The user gives a comma-separated list of tasks
- The user explicitly asks for a todo list

Skip it for single tasks, Q&A, and anything you can finish in one or two straightforward operations — tracking adds friction without value.

- `content`: imperative ("Fix authentication bug")
- `activeForm`: present continuous ("Fixing authentication bug")

Mark exactly one task `in_progress` at a time. Mark `completed` immediately on finish — don't batch. Don't mark completed if tests fail or implementation is partial. Update or remove tasks as the work changes.
