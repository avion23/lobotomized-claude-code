<!--
name: 'Tool Result: Built-in gh Search PRs filter-list example'
description: >-
  Instead-of line in the built-in gh refusal for `gh search prs` (proxy refuses
  search): gh api '${}/pulls?state=all&per_page=100'  # ${}: filter a list
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_SEARCH_PRS_FILTER_LIST_EXAMPLE_VAR_0
  - TOOL_RESULT_BASH_BUILTIN_GH_SEARCH_PRS_FILTER_LIST_EXAMPLE_VAR_1
-->
gh api '${TOOL_RESULT_BASH_BUILTIN_GH_SEARCH_PRS_FILTER_LIST_EXAMPLE_VAR_0}/pulls?state=all&per_page=100'  # ${TOOL_RESULT_BASH_BUILTIN_GH_SEARCH_PRS_FILTER_LIST_EXAMPLE_VAR_1}: filter a list
