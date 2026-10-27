<!--
name: Worktree creation promisor fetch failed
description: >-
  Error that objects for a commit could not be fetched from the promisor remote
  of a partial clone
ccVersion: 2.1.310
variables:
  - DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_0
  - DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_1
  - DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_2
  - DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_3
  - DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_4
  - DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_5
-->
This repository is a partial clone, and ${DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_0.length===1?"an object":`${DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_0.length} objects`} needed for commit ${DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_1} could not be fetched from its promisor remote ${DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_2(DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_3)} before checking it out (Claude Code checks worktrees out with git's on-demand fetching switched off). Check that the remote is reachable (${DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_4(DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_3)?`for example "git fetch ${DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_3}"`:'run "git remote -v" to see which remotes are configured'}) and try again. ${DATA_WORKTREE_CREATION_PROMISOR_FETCH_FAILED_ERROR_VAR_5}
