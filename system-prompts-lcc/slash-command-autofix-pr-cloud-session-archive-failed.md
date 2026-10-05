<!--
name: 'Autofix PR: cloud session archive failed'
description: >-
  Tells the model the earlier cloud session couldn't be archived and may still
  be working the PR, with a link to stop it
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_AUTOFIX_PR_CLOUD_SESSION_ARCHIVE_FAILED_VAR_0
  - SLASH_COMMAND_AUTOFIX_PR_CLOUD_SESSION_ARCHIVE_FAILED_VAR_1
-->
The cloud session started for it couldn't be archived and may still work on the PR. Stop it here: ${SLASH_COMMAND_AUTOFIX_PR_CLOUD_SESSION_ARCHIVE_FAILED_VAR_0(SLASH_COMMAND_AUTOFIX_PR_CLOUD_SESSION_ARCHIVE_FAILED_VAR_1.id,void 0,{from:"cli"})}
