<!--
name: 'cmd deletion blocked: named protected path'
description: >-
  The cmd.exe variant of the bash dangerous-op deny message naming the specific
  protected path the command targets, with an optional reason clause.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_BASH_DANGEROUS_OP_CMD_NAMED_PROTECTED_PATH_VAR_0
  - TOOL_RESULT_BASH_DANGEROUS_OP_CMD_NAMED_PROTECTED_PATH_VAR_1
  - TOOL_RESULT_BASH_DANGEROUS_OP_CMD_NAMED_PROTECTED_PATH_VAR_2
  - TOOL_RESULT_BASH_DANGEROUS_OP_CMD_NAMED_PROTECTED_PATH_VAR_3
-->
cmd's ${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_NAMED_PROTECTED_PATH_VAR_0} on '${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_NAMED_PROTECTED_PATH_VAR_1}' is blocked because${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_NAMED_PROTECTED_PATH_VAR_2===""?"":`, ${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_NAMED_PROTECTED_PATH_VAR_2},`} it targets '${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_NAMED_PROTECTED_PATH_VAR_3.path}', which no command may remove.
