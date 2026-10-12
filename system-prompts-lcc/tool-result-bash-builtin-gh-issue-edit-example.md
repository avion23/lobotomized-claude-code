<!--
name: 'Tool Result: Built-in gh Issue edit example'
description: >-
  Instead-of line in the built-in gh refusal for `gh issue edit`: gh api -X
  PATCH ${}/issues/<number> -f title='<title>' -f body='<text>'
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_ISSUE_EDIT_EXAMPLE_VAR_0
-->
gh api -X PATCH ${TOOL_RESULT_BASH_BUILTIN_GH_ISSUE_EDIT_EXAMPLE_VAR_0}/issues/<number> -f title='<title>' -f body='<text>'
