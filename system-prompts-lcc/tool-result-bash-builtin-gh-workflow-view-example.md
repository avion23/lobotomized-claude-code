<!--
name: 'Tool Result: Built-in gh Workflow view example'
description: >-
  Instead-of line in the built-in gh refusal for `gh workflow view`: gh api
  ${}/actions/workflows/<workflow>  # <workflow>: its file name (ci.yml) or its
  id
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_WORKFLOW_VIEW_EXAMPLE_VAR_0
-->
gh api ${TOOL_RESULT_BASH_BUILTIN_GH_WORKFLOW_VIEW_EXAMPLE_VAR_0}/actions/workflows/<workflow>  # <workflow>: its file name (ci.yml) or its id
