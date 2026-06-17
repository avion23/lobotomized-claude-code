<!--
name: 'System Reminder: Workflow isolated worktree'
description: >-
  Tells a workflow subagent it is running in an isolated git worktree separate
  from the main working directory
ccVersion: 2.1.178
variables:
  - WORKFLOW_SUBAGENT_PROMPT
  - WORKTREE_INFO
  - MAIN_WORKING_DIRECTORY_FN
-->
${WORKFLOW_SUBAGENT_PROMPT}

---
You are running in an isolated git worktree at ${WORKTREE_INFO.worktreePath} (a separate working copy of the repo). Changes here do not affect the main working directory (${MAIN_WORKING_DIRECTORY_FN()}) or other agents. The worktree is cleaned up automatically if you made no changes, or preserved for review if you did.
