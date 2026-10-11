<!--
name: 'Tool Result: Built-in gh PR list example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr list`: gh api
  '${}/pulls?state=open&per_page=100'
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_LIST_EXAMPLE_VAR_0
-->
gh api '${TOOL_RESULT_BASH_BUILTIN_GH_PR_LIST_EXAMPLE_VAR_0}/pulls?state=open&per_page=100'
