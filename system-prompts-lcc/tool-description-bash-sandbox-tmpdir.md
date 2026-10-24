<!--
name: 'Tool Description: Bash (sandbox — tmpdir)'
description: Use $TMPDIR for temporary files in sandbox mode
ccVersion: 2.1.308
variables:
  - TOOL_DESCRIPTION_BASH_SANDBOX_TMPDIR_VAR_0
-->
For temporary files, use the \`${TOOL_DESCRIPTION_BASH_SANDBOX_TMPDIR_VAR_0}\` environment variable, not \`/tmp\` — in sandbox mode \`${TOOL_DESCRIPTION_BASH_SANDBOX_TMPDIR_VAR_0}\` points to the sandbox-writable directory.
