<!--
name: 'System Reminder: Attached machine could not be reached (asleep)'
description: >-
  Follows the could-not-be-reached notice for the asleep case, with what to tell
  the user and barring further calls
ccVersion: 2.1.304
variables:
  - COULD_NOT_BE_REACHED_NOTICE
  - REMOTE_MACHINE_NAME
  - AWAY_UNTIL_CONDITION
  - RECHECK_ON_REQUEST_ENDING
-->
${COULD_NOT_BE_REACHED_NOTICE} Waking the computer is all the user needs to do to bring ${REMOTE_MACHINE_NAME} back. Do not call ${REMOTE_MACHINE_NAME} again ${AWAY_UNTIL_CONDITION}: do the rest of the task without ${REMOTE_MACHINE_NAME}, and tell the user what is blocked.${RECHECK_ON_REQUEST_ENDING}
