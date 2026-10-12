<!--
name: 'Tool Result: Built-in gh PR review threads example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr view` (review threads):
  gh api ${}/pulls/<number>/ccr/review_threads  # its review threads
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_REVIEW_THREADS_EXAMPLE_VAR_0
-->
gh api ${TOOL_RESULT_BASH_BUILTIN_GH_PR_REVIEW_THREADS_EXAMPLE_VAR_0}/pulls/<number>/ccr/review_threads  # its review threads
