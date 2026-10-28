<!--
name: 'Tool Result: Remote tool file rules unread (cannot ask)'
description: >-
  Refusal when the session cannot tell which files a remote command opens and
  cannot ask
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_CANNOT_ASK_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_CANNOT_ASK_VAR_1
  - TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_CANNOT_ASK_VAR_2
-->
This session cannot tell which files a ${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_CANNOT_ASK_VAR_0} command opens on ${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_CANNOT_ASK_VAR_1}, so it cannot check the command against its permission rules for the file tools (${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_CANNOT_ASK_VAR_2}), and this context cannot ask. A file tool's call there is checked against those rules.
