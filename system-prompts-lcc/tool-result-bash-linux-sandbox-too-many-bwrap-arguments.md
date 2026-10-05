<!--
name: 'Tool Result: Linux Sandbox Too Many Bwrap Arguments'
description: >-
  Error surfaced when the Bash tool's Linux sandbox profile expands to more
  bwrap arguments than bwrap accepts, explaining the mount/env-var budget so the
  command can be narrowed.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_0
  - TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_1
-->
Sandbox profile has ${TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_0.length} bwrap arguments and bwrap accepts at most ${TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_1} (about ${TOOL_RESULT_BASH_LINUX_SANDBOX_TOO_MANY_BWRAP_ARGUMENTS_VAR_1/3} mounts); reduce what the configuration expands to: each path takes about three arguments, each environment variable two
