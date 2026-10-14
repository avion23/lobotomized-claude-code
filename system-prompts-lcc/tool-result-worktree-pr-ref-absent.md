<!--
name: 'Worktree PR: ref absent'
description: origin has no PR ref; a look-alike ref was fetched instead.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_WORKTREE_PR_REF_ABSENT_VAR_0
  - TOOL_RESULT_WORKTREE_PR_REF_ABSENT_VAR_1
-->
origin has no ref ${TOOL_RESULT_WORKTREE_PR_REF_ABSENT_VAR_0}; a branch, tag or other ref named like it was fetched instead, which is not pull or merge request #${TOOL_RESULT_WORKTREE_PR_REF_ABSENT_VAR_1.prNumber}. Check the number, and that origin is the repository #${TOOL_RESULT_WORKTREE_PR_REF_ABSENT_VAR_1.prNumber} belongs to; if both are right, that ref has to be deleted from origin first.
