<!--
name: 'Tool Result: Built-in gh Run jobs example'
description: >-
  Instead-of line in the built-in gh refusal for `gh run view` (jobs and steps):
  gh api ${}/actions/runs/<run-id>/jobs  # its jobs and their steps
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_RUN_JOBS_EXAMPLE_VAR_0
-->
gh api ${TOOL_RESULT_BASH_BUILTIN_GH_RUN_JOBS_EXAMPLE_VAR_0}/actions/runs/<run-id>/jobs  # its jobs and their steps
