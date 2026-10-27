<!--
name: Worktree creation unsafe promisor remote error
description: >-
  Error text explaining that missing objects of a partial clone could not be
  pre-fetched because the promisor remote has an option-like name or no URL, and
  directing a check of the remote sections and extensions.partialclone setting
ccVersion: 2.1.310
variables:
  - FORMAT_PROMISOR_REMOTE_NAME_FN
  - PROMISOR_REMOTE_NAMES
  - MISSING_OBJECT_IDS
  - BASE_COMMIT_SHORT_SHA
-->
This repository is a partial clone, but its promisor remote ${FORMAT_PROMISOR_REMOTE_NAME_FN(PROMISOR_REMOTE_NAMES[0])} cannot be fetched from safely (its name begins with "-", which git would read as an option, or it has no URL in the repository's git config), so the ${MISSING_OBJECT_IDS.length===1?"object":`${MISSING_OBJECT_IDS.length} objects`} needed for commit ${BASE_COMMIT_SHORT_SHA} could not be fetched. Look through the [remote "…"] sections and the extensions.partialclone line in that config, and in any file it includes, for a remote you did not set up; correct or remove it, then try again.
