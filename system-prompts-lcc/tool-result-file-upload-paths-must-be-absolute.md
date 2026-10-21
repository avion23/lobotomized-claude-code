<!--
name: 'Tool Result: File upload paths must be absolute'
description: Refusal when file_upload paths are not absolute as this session sees them
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_FILE_UPLOAD_PATHS_MUST_BE_ABSOLUTE_VAR_0
  - TOOL_RESULT_FILE_UPLOAD_PATHS_MUST_BE_ABSOLUTE_VAR_1
-->
Cannot upload "${TOOL_RESULT_FILE_UPLOAD_PATHS_MUST_BE_ABSOLUTE_VAR_0(TOOL_RESULT_FILE_UPLOAD_PATHS_MUST_BE_ABSOLUTE_VAR_1)}": file_upload \`paths\` must be absolute paths as this session sees them (for example /sessions/… in a Cowork VM, or a drive-letter path on Windows).
