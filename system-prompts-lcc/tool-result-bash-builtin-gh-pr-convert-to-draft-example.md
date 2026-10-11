<!--
name: 'Tool Result: Built-in gh PR convert to draft example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr ready --undo`: gh api -X
  POST ${}/pulls/<number>/ccr/convert_to_draft  # --undo
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_CONVERT_TO_DRAFT_EXAMPLE_VAR_0
-->
gh api -X POST ${TOOL_RESULT_BASH_BUILTIN_GH_PR_CONVERT_TO_DRAFT_EXAMPLE_VAR_0}/pulls/<number>/ccr/convert_to_draft  # --undo
