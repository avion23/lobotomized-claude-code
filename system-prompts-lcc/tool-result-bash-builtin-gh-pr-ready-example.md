<!--
name: 'Tool Result: Built-in gh PR ready for review example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr ready`: gh api -X POST
  ${}/pulls/<number>/ccr/ready_for_review
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_READY_EXAMPLE_VAR_0
-->
gh api -X POST ${TOOL_RESULT_BASH_BUILTIN_GH_PR_READY_EXAMPLE_VAR_0}/pulls/<number>/ccr/ready_for_review
