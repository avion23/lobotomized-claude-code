<!--
name: Worktree creation too many missing objects
description: Error that a partial-clone commit needs too many missing objects to fetch
ccVersion: 2.1.310
variables:
  - DATA_WORKTREE_CREATION_PARTIAL_CLONE_TOO_MANY_OBJECTS_ERROR_VAR_0
-->
This repository is a partial clone, and commit ${DATA_WORKTREE_CREATION_PARTIAL_CLONE_TOO_MANY_OBJECTS_ERROR_VAR_0} needs more than about 1.5 million objects it does not have, too many to fetch before checking it out. Limit the worktree with the worktree.sparsePaths setting, or check that commit out once in the main checkout so git fetches them, then try again.
