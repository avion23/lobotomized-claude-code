<!--
name: 'Tool Result: Remote tool refused under managed file deny rules'
description: >-
  Refusal when managed deny rules for file tools are set and the session cannot
  tell which files a remote command opens
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_MANAGED_REFUSED_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_MANAGED_REFUSED_VAR_1
  - TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_MANAGED_REFUSED_VAR_2
-->
This session cannot tell which files a ${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_MANAGED_REFUSED_VAR_0} command opens on ${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_MANAGED_REFUSED_VAR_1}, so it cannot check the command against the deny rules for the file tools in its managed settings (${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_MANAGED_REFUSED_VAR_2}). It sends no ${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_MANAGED_REFUSED_VAR_0} command to ${TOOL_RESULT_REMOTE_TOOL_FILE_RULES_UNREAD_MANAGED_REFUSED_VAR_1} while those rules are set, and the user cannot approve one. A file tool's call there is checked against those rules.
