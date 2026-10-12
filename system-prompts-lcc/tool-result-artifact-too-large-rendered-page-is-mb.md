<!--
name: 'Tool Result: artifact publish — too large: rendered page is …MB (max …MB)'
description: >-
  Artifact page publish preflight diagnostic: too large: rendered page is
  ${.ceil(/1024/1024)}MB (max ${/1024/1024}MB). Emitted through the verified
  route recorded below.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_TOO_LARGE_RENDERED_PAGE_IS_MB_VAR_0
  - TOOL_RESULT_ARTIFACT_TOO_LARGE_RENDERED_PAGE_IS_MB_VAR_1
  - TOOL_RESULT_ARTIFACT_TOO_LARGE_RENDERED_PAGE_IS_MB_VAR_2
-->
too large: rendered page is ${TOOL_RESULT_ARTIFACT_TOO_LARGE_RENDERED_PAGE_IS_MB_VAR_0.ceil(TOOL_RESULT_ARTIFACT_TOO_LARGE_RENDERED_PAGE_IS_MB_VAR_1/1024/1024)}MB (max ${TOOL_RESULT_ARTIFACT_TOO_LARGE_RENDERED_PAGE_IS_MB_VAR_2/1024/1024}MB)
