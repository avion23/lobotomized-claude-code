<!--
name: 'Tool Description: Bash working directory (concise)'
description: >-
  Concise bullet on the working directory, preferring absolute paths and shell
  state not persisting
ccVersion: 2.1.311
variables:
  - TOOL_DESCRIPTION_BASH_WORKING_DIRECTORY_2_VAR_0
-->
- ${TOOL_DESCRIPTION_BASH_WORKING_DIRECTORY_2_VAR_0()} Prefer absolute paths — \`cd\` in a compound command can trigger a permission prompt. Shell state (env vars, functions) does not persist; the shell is initialized from the user's profile.
