<!--
name: 'Tool Result: Built-in gh Workflow run dispatch example'
description: >-
  Instead-of line in the built-in gh refusal for `gh workflow run`: gh api -X
  POST ${}/actions/workflows/<workflow>/dispatches -f ref=<branch>  #
  <workflow>: 
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_WORKFLOW_RUN_EXAMPLE_VAR_0
-->
gh api -X POST ${TOOL_RESULT_BASH_BUILTIN_GH_WORKFLOW_RUN_EXAMPLE_VAR_0}/actions/workflows/<workflow>/dispatches -f ref=<branch>  # <workflow>: its file name (ci.yml) or its id; inputs: -f 'inputs[<name>]=<value>'
