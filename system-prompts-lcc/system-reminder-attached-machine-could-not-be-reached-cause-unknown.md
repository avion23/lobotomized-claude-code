<!--
name: 'System Reminder: Attached machine could not be reached (cause unknown)'
description: >-
  Follows the could-not-be-reached notice for the cause unknown case, with what
  to tell the user and barring further calls
ccVersion: 2.1.304
variables:
  - COULD_NOT_BE_REACHED_NOTICE
  - REMOTE_MACHINE_NAME
  - SAY_WHEN_BACK_CLAUSE
  - AWAY_UNTIL_CONDITION
  - RECHECK_ON_REQUEST_ENDING
-->
${COULD_NOT_BE_REACHED_NOTICE} If Claude is not running on ${REMOTE_MACHINE_NAME}, or is no longer connected to this session, ask the user to check it${SAY_WHEN_BACK_CLAUSE}. Do not call ${REMOTE_MACHINE_NAME} again ${AWAY_UNTIL_CONDITION}: do the rest of the task without ${REMOTE_MACHINE_NAME}, and tell the user what is blocked.${RECHECK_ON_REQUEST_ENDING}
