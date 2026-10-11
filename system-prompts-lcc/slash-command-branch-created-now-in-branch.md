<!--
name: 'Slash Command: /branch — now in the new branch'
description: >-
  /branch result after resuming into the new branch, giving its session id and
  how to return to the original.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_BRANCH_CREATED_NOW_IN_BRANCH_VAR_0
  - SLASH_COMMAND_BRANCH_CREATED_NOW_IN_BRANCH_VAR_1
  - SLASH_COMMAND_BRANCH_CREATED_NOW_IN_BRANCH_VAR_2
  - SLASH_COMMAND_BRANCH_CREATED_NOW_IN_BRANCH_VAR_3
-->
Branched conversation${SLASH_COMMAND_BRANCH_CREATED_NOW_IN_BRANCH_VAR_0}. You are now in the new branch (session ${SLASH_COMMAND_BRANCH_CREATED_NOW_IN_BRANCH_VAR_1}). Use /resume ${SLASH_COMMAND_BRANCH_CREATED_NOW_IN_BRANCH_VAR_2}${SLASH_COMMAND_BRANCH_CREATED_NOW_IN_BRANCH_VAR_3} to return to the original, or run \`claude -r ${SLASH_COMMAND_BRANCH_CREATED_NOW_IN_BRANCH_VAR_2}\` in a new terminal.
