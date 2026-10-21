<!--
name: 'System Reminder: Attached machine could not be reached (went silent)'
description: >-
  Follows the could-not-be-reached notice for the went silent case, with what to
  tell the user and barring further calls
ccVersion: 2.1.304
variables:
  - COULD_NOT_BE_REACHED_NOTICE
  - REMOTE_MACHINE_NAME
  - SAY_WHEN_BACK_CLAUSE
  - AWAY_UNTIL_CONDITION
  - RECHECK_ON_REQUEST_ENDING
-->
${COULD_NOT_BE_REACHED_NOTICE} Most likely Claude on ${REMOTE_MACHINE_NAME} is no longer running (the app was closed, say) or lost its connection, or the computer went to sleep or offline: ask the user to open Claude on ${REMOTE_MACHINE_NAME} again with the computer awake and online${SAY_WHEN_BACK_CLAUSE}. Do not call ${REMOTE_MACHINE_NAME} again ${AWAY_UNTIL_CONDITION}: do the rest of the task without ${REMOTE_MACHINE_NAME}, and tell the user what is blocked.${RECHECK_ON_REQUEST_ENDING}
