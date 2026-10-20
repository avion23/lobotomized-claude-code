<!--
name: 'Tool Result: Remote host ambiguous machine name'
description: >-
  Refusal when a machine name could name this machine or an attached one, asking
  Claude to write the name exactly as listed
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_REMOTE_HOST_AMBIGUOUS_MACHINE_NAME_VAR_0
  - TOOL_RESULT_REMOTE_HOST_AMBIGUOUS_MACHINE_NAME_VAR_1
  - TOOL_RESULT_REMOTE_HOST_AMBIGUOUS_MACHINE_NAME_VAR_2
-->
"${TOOL_RESULT_REMOTE_HOST_AMBIGUOUS_MACHINE_NAME_VAR_0(TOOL_RESULT_REMOTE_HOST_AMBIGUOUS_MACHINE_NAME_VAR_1)}" could name ${TOOL_RESULT_REMOTE_HOST_AMBIGUOUS_MACHINE_NAME_VAR_2.name} or an attached machine; the call did not run. Write the machine's name exactly as this session lists it.
