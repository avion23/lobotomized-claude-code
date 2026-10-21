<!--
name: 'Tool Description: Agent definition and worktree isolation'
description: >-
  Agent types take model, effort and tools from their definition; isolation
  worktree gives an own git worktree
ccVersion: 2.1.301
-->
Each agent type's model, reasoning effort, and tools come from its definition (`.claude/agents/*.md` frontmatter or SDK `agents`). Also take note that `isolation: "worktree"` gives the agent its own git worktree (auto-cleaned if unchanged).
