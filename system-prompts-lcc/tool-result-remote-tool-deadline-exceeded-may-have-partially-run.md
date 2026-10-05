<!--
name: 'Deadline exceeded mid-run, may have partially run'
description: >-
  tool_result message for a call that did not finish within its deadline and was
  stopped; warns it may have partially run and not to retry non-idempotent
  commands blindly.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_DEADLINE_EXCEEDED_MAY_HAVE_PARTIALLY_RUN_VAR_0
-->
The call did not finish within its deadline on ${TOOL_RESULT_REMOTE_TOOL_DEADLINE_EXCEEDED_MAY_HAVE_PARTIALLY_RUN_VAR_0} and was stopped — it may have partially run. Do not retry non-idempotent commands blindly.
