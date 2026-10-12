<!--
name: 'Tool Result: Built-in gh Issue close example'
description: >-
  Instead-of line in the built-in gh refusal for `gh issue close`: gh api -X
  PATCH ${}/issues/<number> -f state=closed
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_ISSUE_CLOSE_EXAMPLE_VAR_0
-->
gh api -X PATCH ${TOOL_RESULT_BASH_BUILTIN_GH_ISSUE_CLOSE_EXAMPLE_VAR_0}/issues/<number> -f state=closed
