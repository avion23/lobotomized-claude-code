<!--
name: Bash disk full output file
description: >-
  Error that the command was not started because the temp volume is full so the
  output file could not be created
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_DISK_FULL_OUTPUT_FILE_VAR_0
  - TOOL_RESULT_BASH_DISK_FULL_OUTPUT_FILE_VAR_1
  - TOOL_RESULT_BASH_DISK_FULL_OUTPUT_FILE_VAR_2
  - TOOL_RESULT_BASH_DISK_FULL_OUTPUT_FILE_VAR_3
  - TOOL_RESULT_BASH_DISK_FULL_OUTPUT_FILE_VAR_4
-->
The command was not started: ${TOOL_RESULT_BASH_DISK_FULL_OUTPUT_FILE_VAR_0} on the volume holding ${TOOL_RESULT_BASH_DISK_FULL_OUTPUT_FILE_VAR_1(TOOL_RESULT_BASH_DISK_FULL_OUTPUT_FILE_VAR_2(),TOOL_RESULT_BASH_DISK_FULL_OUTPUT_FILE_VAR_3())} (Claude Code's temporary directory), so the file that captures command output could not be created there and nothing ran. ${TOOL_RESULT_BASH_DISK_FULL_OUTPUT_FILE_VAR_4}
