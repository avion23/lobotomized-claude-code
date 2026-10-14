<!--
name: 'Worktree PR: other ref unchecked'
description: Could not check whether origin also has the other PR ref; retry.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_WORKTREE_PR_OTHER_REF_UNCHECKED_VAR_0
  - TOOL_RESULT_WORKTREE_PR_OTHER_REF_UNCHECKED_VAR_1
  - TOOL_RESULT_WORKTREE_PR_OTHER_REF_UNCHECKED_VAR_2
-->
fetched ${TOOL_RESULT_WORKTREE_PR_OTHER_REF_UNCHECKED_VAR_0.refspec}, but could not check whether origin also has ${TOOL_RESULT_WORKTREE_PR_OTHER_REF_UNCHECKED_VAR_1.refspec} (${TOOL_RESULT_WORKTREE_PR_OTHER_REF_UNCHECKED_VAR_1.why}). Because origin was not recognised as github.com or gitlab.com, both refs are checked before either is used, so that a pushed look-alike cannot be mistaken for #${TOOL_RESULT_WORKTREE_PR_OTHER_REF_UNCHECKED_VAR_2.prNumber}. Retry.
