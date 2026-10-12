<!--
name: 'Tool Result: Built-in gh Issue create example'
description: >-
  Instead-of line in the built-in gh refusal for `gh issue create`: gh api
  ${}/issues -f title='<title>' -f body='<text>'
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_ISSUE_CREATE_EXAMPLE_VAR_0
-->
gh api ${TOOL_RESULT_BASH_BUILTIN_GH_ISSUE_CREATE_EXAMPLE_VAR_0}/issues -f title='<title>' -f body='<text>'
