<!--
name: 'Tool Result: Tool not loaded, load first'
description: >-
  InputValidationError telling the model to load a deferred tool with ToolSearch
  before calling it
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_TOOL_NOT_LOADED_LOAD_FIRST_VAR_0
  - TOOL_RESULT_TOOL_NOT_LOADED_LOAD_FIRST_VAR_1
-->
InputValidationError: ${TOOL_RESULT_TOOL_NOT_LOADED_LOAD_FIRST_VAR_0} did not run: it was not loaded when it was called. Unless ${TOOL_RESULT_TOOL_NOT_LOADED_LOAD_FIRST_VAR_1} has loaded it since, load it together with the other tools you expect to need, in one ${TOOL_RESULT_TOOL_NOT_LOADED_LOAD_FIRST_VAR_1} call (for example, query "select:${TOOL_RESULT_TOOL_NOT_LOADED_LOAD_FIRST_VAR_0}", with the other names after it, comma-separated). Call it again once that result has come back, not in the same reply.
