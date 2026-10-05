<!--
name: 'cmd deletion blocked: workspace/protected directory'
description: >-
  The cmd.exe variant of the bash dangerous-op deny message for when the target
  path itself (T.path) is the protected path, e.g. the workspace directory.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_BASH_DANGEROUS_OP_CMD_WORKSPACE_DIRECTORY_VAR_0
  - TOOL_RESULT_BASH_DANGEROUS_OP_CMD_WORKSPACE_DIRECTORY_VAR_1
-->
cmd's ${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_WORKSPACE_DIRECTORY_VAR_0} on '${TOOL_RESULT_BASH_DANGEROUS_OP_CMD_WORKSPACE_DIRECTORY_VAR_1.path}' is blocked because no command may remove that path.
