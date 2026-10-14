<!--
name: 'Send file: sign-in expired remedy'
description: >-
  Remedy text telling the model to wait five minutes before retrying a file send
  after sign-in expiry.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_SEND_FILE_CLOUD_SIGN_IN_EXPIRED_REMEDY_VAR_0
-->
an expired sign-in is renewed once this turn has ended and the environment has then run no tool call or ${TOOL_RESULT_SEND_FILE_CLOUD_SIGN_IN_EXPIRED_REMEDY_VAR_0} watch for about five minutes, so do not send again or run sleep now; tell the user to wait at least five minutes without sending anything else in this chat, and then to ask for the file again. If a send after such a wait fails like this too, tell the user instead that sending files may not work in this chat for now
