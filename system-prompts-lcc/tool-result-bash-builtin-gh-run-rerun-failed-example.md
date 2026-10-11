<!--
name: 'Tool Result: Built-in gh Run rerun failed example'
description: >-
  Instead-of line in the built-in gh refusal for `gh run rerun --failed`: gh api
  -X POST ${}/actions/runs/<run-id>/rerun-failed-jobs  # --failed
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_RUN_RERUN_FAILED_EXAMPLE_VAR_0
-->
gh api -X POST ${TOOL_RESULT_BASH_BUILTIN_GH_RUN_RERUN_FAILED_EXAMPLE_VAR_0}/actions/runs/<run-id>/rerun-failed-jobs  # --failed
