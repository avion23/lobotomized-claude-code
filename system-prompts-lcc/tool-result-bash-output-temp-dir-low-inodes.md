<!--
name: Bash output temp dir low inodes
description: Note that the temp directory's volume is nearly out of inodes
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_LOW_INODES_VAR_0
  - TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_LOW_INODES_VAR_1
  - TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_LOW_INODES_VAR_2
-->
Nearly out of inodes: this computer's volume holding ${TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_LOW_INODES_VAR_0} (Claude Code's temporary directory) has ${TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_LOW_INODES_VAR_1.ffree} free inodes, so creating files there may fail and the command may have failed for that reason. ${TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_LOW_INODES_VAR_2}
