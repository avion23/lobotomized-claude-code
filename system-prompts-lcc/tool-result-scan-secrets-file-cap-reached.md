<!--
name: 'scan_secrets: file cap reached'
description: Warning that only the first N files and folders were looked at.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_SCAN_SECRETS_FILE_CAP_REACHED_VAR_0
  - TOOL_RESULT_SCAN_SECRETS_FILE_CAP_REACHED_VAR_1
-->
${TOOL_RESULT_SCAN_SECRETS_FILE_CAP_REACHED_VAR_0.warning} Only the first ${TOOL_RESULT_SCAN_SECRETS_FILE_CAP_REACHED_VAR_1.toLocaleString("en-US")} files and folders were looked at; the rest of the folder was not scanned, and which files it holds is unknown.
