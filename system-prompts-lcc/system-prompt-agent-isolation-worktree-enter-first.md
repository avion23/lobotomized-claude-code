<!--
name: 'System Prompt: isolation worktree, enter first'
description: >-
  Agent configured with isolation: worktree must call EnterWorktree first unless
  already in .claude/worktrees
ccVersion: 2.1.301
-->
This agent is configured with `isolation: worktree`. Please call the EnterWorktree tool as your first action before reading files or running commands, unless your cwd is already under `.claude/worktrees/`. If EnterWorktree fails, continue in place.
