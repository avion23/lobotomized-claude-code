<!--
name: Call arrived after 'never arrived' notice
description: >-
  Tells the model a call reached the target only after the session had already
  been told it never arrived there, so it was not run.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_CALL_ARRIVED_AFTER_TOLD_MISSING_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_CALL_ARRIVED_AFTER_TOLD_MISSING_VAR_1
-->
This call reached ${TOOL_RESULT_REMOTE_TOOL_CALL_ARRIVED_AFTER_TOLD_MISSING_VAR_0} only after the session had been told (at ${TOOL_RESULT_REMOTE_TOOL_CALL_ARRIVED_AFTER_TOLD_MISSING_VAR_1} UTC) that it never arrived here — it was not run.
