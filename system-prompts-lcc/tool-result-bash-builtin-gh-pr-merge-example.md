<!--
name: 'Tool Result: Built-in gh PR merge example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr merge`: gh api -X PUT
  ${}/pulls/<number>/merge -f merge_method=squash
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_MERGE_EXAMPLE_VAR_0
-->
gh api -X PUT ${TOOL_RESULT_BASH_BUILTIN_GH_PR_MERGE_EXAMPLE_VAR_0}/pulls/<number>/merge -f merge_method=squash
