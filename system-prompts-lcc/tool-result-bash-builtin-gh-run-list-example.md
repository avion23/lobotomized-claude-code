<!--
name: 'Tool Result: Built-in gh Run list example'
description: >-
  Instead-of line in the built-in gh refusal for `gh run list`: gh api
  '${}/actions/runs?per_page=20'  # filters: branch=, event=, status=, head_sha=
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_RUN_LIST_EXAMPLE_VAR_0
-->
gh api '${TOOL_RESULT_BASH_BUILTIN_GH_RUN_LIST_EXAMPLE_VAR_0}/actions/runs?per_page=20'  # filters: branch=, event=, status=, head_sha=
