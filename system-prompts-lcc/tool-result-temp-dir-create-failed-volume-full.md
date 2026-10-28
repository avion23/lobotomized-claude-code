<!--
name: Temp dir could not be created
description: >-
  Error that Claude Code's temporary directory could not be created because its
  volume is full, suggesting freeing space or CLAUDE_CODE_TMPDIR
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_TEMP_DIR_CREATE_FAILED_VOLUME_FULL_VAR_0
  - TOOL_RESULT_TEMP_DIR_CREATE_FAILED_VOLUME_FULL_VAR_1
-->
Claude Code's temporary directory ${TOOL_RESULT_TEMP_DIR_CREATE_FAILED_VOLUME_FULL_VAR_0} could not be created: ${TOOL_RESULT_TEMP_DIR_CREATE_FAILED_VOLUME_FULL_VAR_1}. Free space on that volume, or set CLAUDE_CODE_TMPDIR to a directory on another one, then try again.
