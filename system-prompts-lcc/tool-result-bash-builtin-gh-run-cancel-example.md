<!--
name: 'Tool Result: Built-in gh Run cancel example'
description: >-
  Instead-of line in the built-in gh refusal for `gh run cancel`: gh api -X POST
  ${}/actions/runs/<run-id>/cancel
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_RUN_CANCEL_EXAMPLE_VAR_0
-->
gh api -X POST ${TOOL_RESULT_BASH_BUILTIN_GH_RUN_CANCEL_EXAMPLE_VAR_0}/actions/runs/<run-id>/cancel
