<!--
name: 'Tool Result: File attach repo permission rules unreadable'
description: >-
  Error that the cloud environment could not read the repository's permission
  rules, so files were not attached, and Claude should tell the user the
  settings files may need fixing
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_FILE_ATTACH_REPO_RULES_UNREAD_VAR_0
-->
This session's cloud environment could not read the repository's permission rules, so the files were not attached. ${TOOL_RESULT_FILE_ATTACH_REPO_RULES_UNREAD_VAR_0} Retrying won't help: tell the user that .claude/settings.json or .claude/settings.local.json may have to be fixed or removed.
