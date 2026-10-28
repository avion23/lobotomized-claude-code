<!--
name: 'Tool Result: Remote tool file rules unread (ask)'
description: >-
  Ask message when the session cannot tell which files a remote command opens,
  so it cannot check file-tool permission rules
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_ASK_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_ASK_VAR_1
  - TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_ASK_VAR_2
-->
This session cannot tell which files a ${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_ASK_VAR_0} command opens on ${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_ASK_VAR_1}, so it cannot check the command against its permission rules for the file tools (${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_ASK_VAR_2}). Allow it only if it does nothing that those rules are there to stop.
