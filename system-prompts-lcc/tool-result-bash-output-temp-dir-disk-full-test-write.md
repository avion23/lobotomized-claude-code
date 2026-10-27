<!--
name: Bash output temp dir disk full test write
description: Note that a test write beside the output file failed with ENOSPC
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_DISK_FULL_TEST_WRITE_VAR_0
  - TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_DISK_FULL_TEST_WRITE_VAR_1
  - TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_DISK_FULL_TEST_WRITE_VAR_2
-->
Disk full: a test write beside this command's output file, on the volume holding ${TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_DISK_FULL_TEST_WRITE_VAR_0} (Claude Code's temporary directory), failed with ENOSPC (the volume, or the user's quota on it, has no space left), ${TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_DISK_FULL_TEST_WRITE_VAR_1} ${TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_DISK_FULL_TEST_WRITE_VAR_2}
