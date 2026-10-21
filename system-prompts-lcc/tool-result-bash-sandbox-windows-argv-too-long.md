<!--
name: Windows sandbox argv too long
description: >-
  The sandbox command line exceeds the CreateProcessW limit; lists what it
  carries.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_1
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_2
-->
Windows sandbox argv is ~${TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_0} chars (CreateProcessW limit is 32 767). Besides the command itself it carries ${TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_1.denyRead?.TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_2??0} per-command read denies, ${TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_1.denyReadExcept?.TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_2??0} session grants beneath them, ${TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_1.denyWrite?.TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_2??0} write denies and ${TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_1.writeRoots?.TOOL_RESULT_BASH_SANDBOX_WINDOWS_ARGV_TOO_LONG_VAR_2??0} write roots; the command was not run with fewer.
