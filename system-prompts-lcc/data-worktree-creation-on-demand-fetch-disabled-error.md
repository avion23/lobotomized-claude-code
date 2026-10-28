<!--
name: Worktree creation on-demand fetch disabled error
description: >-
  Error text appended when worktree creation needs a missing git object with
  on-demand fetching off, suggesting git archive or git fsck
ccVersion: 2.1.310
variables:
  - DATA_WORKTREE_CREATION_ON_DEMAND_FETCH_DISABLED_ERROR_VAR_0
-->

This checkout ran with git's on-demand fetching switched off, and git needed an object this repository does not have. If the repository is a partial clone, run "git archive -o objects.tar ${DATA_WORKTREE_CREATION_ON_DEMAND_FETCH_DISABLED_ERROR_VAR_0}" (git fetches the commit's missing files — in a sparse checkout, the whole tree's; delete objects.tar afterwards) in its main checkout and try again; otherwise check it with "git fsck".
