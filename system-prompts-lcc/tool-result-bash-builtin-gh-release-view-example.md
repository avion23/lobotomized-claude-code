<!--
name: 'Tool Result: Built-in gh Release view by tag example'
description: >-
  Instead-of line in the built-in gh refusal for `gh release view` / `gh release
  download`: gh api ${}/releases/tags/<tag>
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_BUILTIN_GH_RELEASE_VIEW_EXAMPLE_VAR_0
-->
gh api ${TOOL_RESULT_BASH_BUILTIN_GH_RELEASE_VIEW_EXAMPLE_VAR_0}/releases/tags/<tag>
