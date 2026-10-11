<!--
name: 'Tool result: Claude Design operation HTTP failure'
description: >-
  Error from the Claude Design tool when an operation returns a non-2xx HTTP
  status, with the status and truncated body.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_0
  - TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_1
  - TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_2
  - TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_3
  - TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_4
-->
Claude Design ${TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_0} failed: HTTP ${TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_1.status} ${TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_2(TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_3(TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_1.data)??"",TOOL_RESULT_DESIGN_HTTP_FAILED_VAR_4)}
