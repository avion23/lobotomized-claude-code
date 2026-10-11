<!--
name: 'Tool Result: Built-in gh PR edit example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr edit`: gh api -X PATCH
  ${}/pulls/<number> -f title='<title>' -f body='<text>'
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_EDIT_EXAMPLE_VAR_0
-->
gh api -X PATCH ${TOOL_RESULT_BASH_BUILTIN_GH_PR_EDIT_EXAMPLE_VAR_0}/pulls/<number> -f title='<title>' -f body='<text>'
