<!--
name: 'Tool Result: MCP connector approval conditioned on edited arguments'
description: >-
  MCP connector call error when the retroactive approval came with edited
  arguments that cannot be applied; deny and re-issue the call to change
  arguments.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_MCP_CCR_APPROVAL_EDITED_ARGUMENTS_VAR_0
-->
The approval for ${TOOL_RESULT_MCP_CCR_APPROVAL_EDITED_ARGUMENTS_VAR_0} was conditioned on edited arguments, which can't be applied on this retroactive card. To run with different arguments, deny and re-issue the call.
