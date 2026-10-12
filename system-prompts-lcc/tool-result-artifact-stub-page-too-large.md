<!--
name: 'Tool result: artifact page too large (stub publish)'
description: >-
  Artifact publish refusal when the page exceeds the size limit on the stub
  publish path, giving the page size and the maximum.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_STUB_PAGE_TOO_LARGE_VAR_0
  - TOOL_RESULT_ARTIFACT_STUB_PAGE_TOO_LARGE_VAR_1
  - TOOL_RESULT_ARTIFACT_STUB_PAGE_TOO_LARGE_VAR_2
-->
too large: page is ${TOOL_RESULT_ARTIFACT_STUB_PAGE_TOO_LARGE_VAR_0.ceil(TOOL_RESULT_ARTIFACT_STUB_PAGE_TOO_LARGE_VAR_1/1024/1024)}MB (max ${TOOL_RESULT_ARTIFACT_STUB_PAGE_TOO_LARGE_VAR_2/1024/1024}MB)
