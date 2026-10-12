<!--
name: 'Tool Result: Built-in gh PR auto-merge example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr merge --auto`: gh api -X
  PUT ${}/pulls/<number>/ccr/auto_merge -f merge_method=squash  # --auto; -X
  DELET
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_AUTO_MERGE_EXAMPLE_VAR_0
-->
gh api -X PUT ${TOOL_RESULT_BASH_BUILTIN_GH_PR_AUTO_MERGE_EXAMPLE_VAR_0}/pulls/<number>/ccr/auto_merge -f merge_method=squash  # --auto; -X DELETE cancels it
