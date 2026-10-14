<!--
name: 'Tool Result: Send message elevated session reachable via session tool'
description: >-
  Says the target may be reachable with the session service's own send tool and
  gives its session id
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_SEND_MESSAGE_REMOTE_CONTROL_ELEVATED_SESSION_TOOL_HINT_VAR_0
  - TOOL_RESULT_SEND_MESSAGE_REMOTE_CONTROL_ELEVATED_SESSION_TOOL_HINT_VAR_1
  - TOOL_RESULT_SEND_MESSAGE_REMOTE_CONTROL_ELEVATED_SESSION_TOOL_HINT_VAR_2
-->
${TOOL_RESULT_SEND_MESSAGE_REMOTE_CONTROL_ELEVATED_SESSION_TOOL_HINT_VAR_0} ${TOOL_RESULT_SEND_MESSAGE_REMOTE_CONTROL_ELEVATED_SESSION_TOOL_HINT_VAR_1}. This target may be reachable with ${TOOL_RESULT_SEND_MESSAGE_REMOTE_CONTROL_ELEVATED_SESSION_TOOL_HINT_VAR_2.sendTool}, the session service's own tool, if your user has allowed this cloud session to reach that computer; that session's id there is "${TOOL_RESULT_SEND_MESSAGE_REMOTE_CONTROL_ELEVATED_SESSION_TOOL_HINT_VAR_2.sessionId}". A tool of that name on any other server is not it.
