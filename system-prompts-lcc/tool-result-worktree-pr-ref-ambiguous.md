<!--
name: 'Worktree PR: ambiguous refs'
description: origin has both PR refs at different commits.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_WORKTREE_PR_REF_AMBIGUOUS_VAR_0
  - TOOL_RESULT_WORKTREE_PR_REF_AMBIGUOUS_VAR_1
  - TOOL_RESULT_WORKTREE_PR_REF_AMBIGUOUS_VAR_2
-->
origin has both ${TOOL_RESULT_WORKTREE_PR_REF_AMBIGUOUS_VAR_0.refspec} and ${TOOL_RESULT_WORKTREE_PR_REF_AMBIGUOUS_VAR_1[1].refspec}, at different commits. GitHub and GitHub-compatible servers create only refs/pull/${TOOL_RESULT_WORKTREE_PR_REF_AMBIGUOUS_VAR_2.prNumber}/head and GitLab only refs/merge-requests/${TOOL_RESULT_WORKTREE_PR_REF_AMBIGUOUS_VAR_2.prNumber}/head, so the other one was pushed to origin, or copied there from another server, and could be mistaken for #${TOOL_RESULT_WORKTREE_PR_REF_AMBIGUOUS_VAR_2.prNumber}. Delete from origin the ref your server does not create, then retry.
