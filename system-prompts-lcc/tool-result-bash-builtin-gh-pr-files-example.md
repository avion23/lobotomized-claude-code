<!--
name: 'Tool Result: Built-in gh PR files example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr diff` (per-file
  patches): gh api ${}/pulls/<number>/files  # one patch per file
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_FILES_EXAMPLE_VAR_0
-->
gh api ${TOOL_RESULT_BASH_BUILTIN_GH_PR_FILES_EXAMPLE_VAR_0}/pulls/<number>/files  # one patch per file
