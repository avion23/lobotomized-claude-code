<!--
name: 'Loop: send update before wakeup tool call'
description: 'Branch of Nln()''s second clause, same confirmed steps34 consumer.'
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_LOOP_PREARM_SEND_BEFORE_TOOL_CALL_VAR_0
  - TOOL_RESULT_LOOP_PREARM_SEND_BEFORE_TOOL_CALL_VAR_1
-->
 ${TOOL_RESULT_LOOP_PREARM_SEND_BEFORE_TOOL_CALL_VAR_0?"Send":"Write"} it immediately BEFORE calling ${TOOL_RESULT_LOOP_PREARM_SEND_BEFORE_TOOL_CALL_VAR_1} — on this model the turn ends as soon as that tool returns, so an update after the call never goes out.
