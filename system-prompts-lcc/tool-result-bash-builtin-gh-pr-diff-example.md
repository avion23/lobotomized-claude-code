<!--
name: 'Tool Result: Built-in gh PR diff example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr diff`: gh api
  ${}/pulls/<number> -H 'Accept: application/vnd.github.diff'
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_DIFF_EXAMPLE_VAR_0
-->
gh api ${TOOL_RESULT_BASH_BUILTIN_GH_PR_DIFF_EXAMPLE_VAR_0}/pulls/<number> -H 'Accept: application/vnd.github.diff'
