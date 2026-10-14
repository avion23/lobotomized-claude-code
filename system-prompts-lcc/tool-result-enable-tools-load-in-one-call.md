<!--
name: 'Enable: load tools in one call'
description: Load the needed tools in one ToolSearch call and wait for the result.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_ENABLE_TOOLS_LOAD_IN_ONE_CALL_VAR_0
  - TOOL_RESULT_ENABLE_TOOLS_LOAD_IN_ONE_CALL_VAR_1
-->
${TOOL_RESULT_ENABLE_TOOLS_LOAD_IN_ONE_CALL_VAR_0}: load the ones you expect to need in one ${TOOL_RESULT_ENABLE_TOOLS_LOAD_IN_ONE_CALL_VAR_1} call (for example, query "select:<name>[,<name>...]"), and use them once that result has come back, not in the same reply
