<!--
name: 'cmd deletion blocked: targets a critical directory'
description: >-
  The cmd.exe-path variant of the bash dangerous-op deny decision, returned by
  ke(b, message) when a Windows cmd delete/remove verb targets a drive root, a
  folder directly under one, or the home folder; the {behavior:'ask',message}
  this composes becomes the tool_result the model reads on denial (same family
  as the existing tool-result-bash-dangerous-op-* rm-protection messages).
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_BASH_DANGEROUS_OP_CMD_CRITICAL_DIRECTORY_REASON_VAR_0
  - TOOL_RESULT_BASH_DANGEROUS_OP_CMD_CRITICAL_DIRECTORY_REASON_VAR_1
  - TOOL_RESULT_BASH_DANGEROUS_OP_CMD_CRITICAL_DIRECTORY_REASON_VAR_2
-->
cmd's ${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_CRITICAL_DIRECTORY_REASON_VAR_0} on '${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_CRITICAL_DIRECTORY_REASON_VAR_1}' is blocked because, ${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_CRITICAL_DIRECTORY_REASON_VAR_2}, it targets a path that no command may remove: a drive root, a folder directly under one, or the home folder.
