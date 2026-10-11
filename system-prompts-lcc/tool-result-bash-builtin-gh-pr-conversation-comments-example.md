<!--
name: 'Tool Result: Built-in gh PR conversation comments example'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr view` (conversation
  comments): gh api ${}/issues/<number>/comments  # its conversation comments
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_PR_CONVERSATION_COMMENTS_EXAMPLE_VAR_0
-->
gh api ${TOOL_RESULT_BASH_BUILTIN_GH_PR_CONVERSATION_COMMENTS_EXAMPLE_VAR_0}/issues/<number>/comments  # its conversation comments
