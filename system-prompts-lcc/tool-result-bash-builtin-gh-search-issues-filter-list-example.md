<!--
name: 'Tool Result: Built-in gh Search issues filter-list example'
description: >-
  Instead-of line in the built-in gh refusal for `gh search issues` (proxy
  refuses search): gh api '${}/issues?state=all&labels=<label>'  # ${}: filter a
  list
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_SEARCH_ISSUES_FILTER_LIST_EXAMPLE_VAR_0
  - TOOL_RESULT_BASH_BUILTIN_GH_SEARCH_ISSUES_FILTER_LIST_EXAMPLE_VAR_1
-->
gh api '${TOOL_RESULT_BASH_BUILTIN_GH_SEARCH_ISSUES_FILTER_LIST_EXAMPLE_VAR_0}/issues?state=all&labels=<label>'  # ${TOOL_RESULT_BASH_BUILTIN_GH_SEARCH_ISSUES_FILTER_LIST_EXAMPLE_VAR_1}: filter a list
