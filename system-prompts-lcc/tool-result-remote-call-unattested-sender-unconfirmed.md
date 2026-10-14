<!--
name: 'Tool Result: Remote call sender unconfirmed'
description: >-
  Says the target got no confirmation this session is the sender and asks to
  tell the user and continue without it
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_REMOTE_CALL_UNATTESTED_SENDER_UNCONFIRMED_VAR_0
  - TOOL_RESULT_REMOTE_CALL_UNATTESTED_SENDER_UNCONFIRMED_VAR_1
-->
${TOOL_RESULT_REMOTE_CALL_UNATTESTED_SENDER_UNCONFIRMED_VAR_0} Retrying, reconnecting ${TOOL_RESULT_REMOTE_CALL_UNATTESTED_SENDER_UNCONFIRMED_VAR_1} or changing a setting on it is unlikely to fix this, and a new session is unlikely to help: ${TOOL_RESULT_REMOTE_CALL_UNATTESTED_SENDER_UNCONFIRMED_VAR_1} got no confirmation it could read from Anthropic's service that this session is the sender. Tell the user that, ask them to report it to Anthropic, and continue without ${TOOL_RESULT_REMOTE_CALL_UNATTESTED_SENDER_UNCONFIRMED_VAR_1}.
