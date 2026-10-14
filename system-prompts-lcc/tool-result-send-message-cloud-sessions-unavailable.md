<!--
name: 'Tool Result: SendMessage cloud sessions unavailable'
description: >-
  Says the account's other sessions could not be checked and to retry instead of
  another tool
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_SEND_MESSAGE_CLOUD_SESSIONS_UNAVAILABLE_VAR_0
  - TOOL_RESULT_SEND_MESSAGE_CLOUD_SESSIONS_UNAVAILABLE_VAR_1
  - TOOL_RESULT_SEND_MESSAGE_CLOUD_SESSIONS_UNAVAILABLE_VAR_2
-->

Your account's other sessions (Remote Control and cloud) could not be checked just now, so they were not searched. If '${TOOL_RESULT_SEND_MESSAGE_CLOUD_SESSIONS_UNAVAILABLE_VAR_0.to}' is one, retry${TOOL_RESULT_SEND_MESSAGE_CLOUD_SESSIONS_UNAVAILABLE_VAR_1?` (or run ${TOOL_RESULT_SEND_MESSAGE_CLOUD_SESSIONS_UNAVAILABLE_VAR_2} first)`:""}; do not look for another tool to send it with.
