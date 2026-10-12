<!--
name: 'Tool Result: Built-in gh PR create example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr create`: gh api
  ${}/pulls -f title='<title>' -f head='<branch>' -f base='<base branch>' -f
  body='<t
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_CREATE_EXAMPLE_VAR_0
-->
gh api ${TOOL_RESULT_BASH_BUILTIN_GH_PR_CREATE_EXAMPLE_VAR_0}/pulls -f title='<title>' -f head='<branch>' -f base='<base branch>' -f body='<text>'  # a draft: add -F draft=true
