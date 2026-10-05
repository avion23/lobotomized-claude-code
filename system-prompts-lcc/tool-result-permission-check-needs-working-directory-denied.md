<!--
name: Permission check denied — no working directory for this session
description: >-
  Deny-decision message returned from a tool's checkPermissions-adjacent
  exception path (t0e, invoked from hWt's catch block) when the session has no
  working directory to check against; becomes the tool_result content the model
  sees when its call is denied.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_PERMISSION_CHECK_NEEDS_WORKING_DIRECTORY_DENIED_VAR_0
-->
The ${TOOL_RESULT_PERMISSION_CHECK_NEEDS_WORKING_DIRECTORY_DENIED_VAR_0.name} permission check needs a working directory, and this session has none, so the call is denied. A retry is denied the same way.
