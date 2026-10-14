<!--
name: 'Tool Result: Remote host no answer assume away'
description: >-
  Tells the model to assume the user is away, finish only approval-free work and
  report the calls not run
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_REMOTE_HOST_NO_ANSWER_ASSUME_AWAY_VAR_0
  - TOOL_RESULT_REMOTE_HOST_NO_ANSWER_ASSUME_AWAY_VAR_1
-->
Assume the user is away: a further call to ${TOOL_RESULT_REMOTE_HOST_NO_ANSWER_ASSUME_AWAY_VAR_0} that needs approval, whether this one again, another command or a file edit, would wait up to ${TOOL_RESULT_REMOTE_HOST_NO_ANSWER_ASSUME_AWAY_VAR_1} and close the same way. Finish only what needs no approval on ${TOOL_RESULT_REMOTE_HOST_NO_ANSWER_ASSUME_AWAY_VAR_0}, then stop and tell the user which calls were not run
