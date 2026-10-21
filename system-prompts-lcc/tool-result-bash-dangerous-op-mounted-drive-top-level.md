<!--
name: 'Tool Result: Bash dangerous op on mounted drive or top level'
description: >-
  Ask message when an rm would remove a mounted drive, the folder holding
  mounted drives, or a top-level entry of a drive, requiring explicit approval
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_BASH_DANGEROUS_OP_MOUNTED_DRIVE_TOP_LEVEL_VAR_0
  - TOOL_RESULT_BASH_DANGEROUS_OP_MOUNTED_DRIVE_TOP_LEVEL_VAR_1
-->
Dangerous ${TOOL_RESULT_BASH_DANGEROUS_OP_MOUNTED_DRIVE_TOP_LEVEL_VAR_0} operation detected: '${TOOL_RESULT_BASH_DANGEROUS_OP_MOUNTED_DRIVE_TOP_LEVEL_VAR_1}'

This command would remove a mounted drive, the folder that holds mounted drives, or a file or folder at the top level of a drive. This requires explicit approval and cannot be auto-allowed by permission rules.

If you meant something deeper inside, name it by its full path.
