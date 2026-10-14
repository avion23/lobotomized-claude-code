<!--
name: 'Worktree PR: FETCH_HEAD overwritten'
description: 'FETCH_HEAD does not record the ref, likely overwritten by a concurrent fetch.'
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_WORKTREE_PR_FETCH_HEAD_OVERWRITTEN_VAR_0
  - TOOL_RESULT_WORKTREE_PR_FETCH_HEAD_OVERWRITTEN_VAR_1
-->
the fetch succeeded, but FETCH_HEAD does not record ${TOOL_RESULT_WORKTREE_PR_FETCH_HEAD_OVERWRITTEN_VAR_0} from ${TOOL_RESULT_WORKTREE_PR_FETCH_HEAD_OVERWRITTEN_VAR_1}, most likely because another git fetch in this repository overwrote it at the same moment. Run the command again.
