<!--
name: Unknown tool name — deferred successor hint
description: >-
  Appended to an unrecognized-tool-name error: tells the model to call the
  correctly-named tool, loading it first via a ToolSearch-style select:<name>
  query if not yet loaded.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_UNKNOWN_TOOL_NAME_DEFERRED_SUCCESSOR_VAR_0
  - TOOL_RESULT_UNKNOWN_TOOL_NAME_DEFERRED_SUCCESSOR_VAR_1
-->
. Call ${TOOL_RESULT_UNKNOWN_TOOL_NAME_DEFERRED_SUCCESSOR_VAR_0.name} instead, loading it first with ${TOOL_RESULT_UNKNOWN_TOOL_NAME_DEFERRED_SUCCESSOR_VAR_1} query "select:${TOOL_RESULT_UNKNOWN_TOOL_NAME_DEFERRED_SUCCESSOR_VAR_0.name}" if it is not loaded yet.
