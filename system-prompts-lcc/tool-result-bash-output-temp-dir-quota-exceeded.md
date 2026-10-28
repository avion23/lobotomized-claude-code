<!--
name: Bash output temp dir quota exceeded
description: >-
  Note appended to a failed Bash command that a test write in Claude Code's temp
  dir failed with EDQUOT
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_QUOTA_EXCEEDED_VAR_0
  - TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_QUOTA_EXCEEDED_VAR_1
-->
Disk quota used up: a test write beside this command's output file, on the volume holding ${TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_QUOTA_EXCEEDED_VAR_0} (Claude Code's temporary directory), failed with EDQUOT, so ${TOOL_RESULT_BASH_OUTPUT_TEMP_DIR_QUOTA_EXCEEDED_VAR_1} and its own writes may have failed with "Disk quota exceeded". Delete files there that are no longer needed, or restart Claude Code with CLAUDE_CODE_TMPDIR set to a directory on another volume, then retry. If this is the user's own computer, tell them before deleting anything to make room.
