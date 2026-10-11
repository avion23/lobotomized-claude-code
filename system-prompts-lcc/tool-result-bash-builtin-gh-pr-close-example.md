<!--
name: 'Tool Result: Built-in gh PR close example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr close`: gh api -X PATCH
  ${}/pulls/<number> -f state=closed
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_CLOSE_EXAMPLE_VAR_0
-->
gh api -X PATCH ${TOOL_RESULT_BASH_BUILTIN_GH_PR_CLOSE_EXAMPLE_VAR_0}/pulls/<number> -f state=closed
