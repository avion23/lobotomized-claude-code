<!--
name: 'Tool Result: Bash Linux sandbox bwrap arguments breakdown'
description: >-
  Explains how many bwrap arguments are built-in write protection for shell/tool
  settings and git hooks/config versus what the configuration expands to, and
  how to reduce them
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_BASH_LINUX_SANDBOX_BWRAP_ARGUMENTS_BREAKDOWN_VAR_0
  - TOOL_RESULT_BASH_LINUX_SANDBOX_BWRAP_ARGUMENTS_BREAKDOWN_VAR_1
-->
${TOOL_RESULT_BASH_LINUX_SANDBOX_BWRAP_ARGUMENTS_BREAKDOWN_VAR_0.mandatoryDenyArgs} of its arguments are built-in write protection, in no list of the configuration: shell and tool settings and each git repository's hooks and config, in and below the working directory, and the directories holding them. For fewer, run from a directory with fewer repositories in it, or allow writing to fewer of them; a lower mandatoryDenySearchDepth leaves the deeper ones unprotected. The other ${TOOL_RESULT_BASH_LINUX_SANDBOX_BWRAP_ARGUMENTS_BREAKDOWN_VAR_1.length-TOOL_RESULT_BASH_LINUX_SANDBOX_BWRAP_ARGUMENTS_BREAKDOWN_VAR_0.mandatoryDenyArgs} are what the configuration expands to: each path takes about three arguments, each environment variable two
