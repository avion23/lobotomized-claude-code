<!--
name: 'Tool Result: Bash Dangerous Op — cmd variables replaced reach a protected path'
description: >-
  Explains that, with cmd's %NAME% variables substituted (and PowerShell $
  variables empty), the command targets a non-removable path.
ccVersion: 2.1.296
variables:
  - >-
    TOOL_RESULT_BASH_DANGEROUS_OP_CMD_CRITICAL_DIRECTORY_VARIABLES_REPLACED_VAR_0
-->
with cmd's %NAME% variables replaced${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_CRITICAL_DIRECTORY_VARIABLES_REPLACED_VAR_0!==null?" and PowerShell's $ variables empty":""}
