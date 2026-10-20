<!--
name: 'System Reminder: Attached machine could not be reached (busy)'
description: >-
  Follows the could-not-be-reached notice for the busy case, with what to tell
  the user and barring further calls
ccVersion: 2.1.304
variables:
  - COULD_NOT_BE_REACHED_NOTICE
  - REMOTE_MACHINE_NAME
  - IS_RETURN_NOTED
  - AWAY_UNTIL_CONDITION
  - RECHECK_ON_REQUEST_ENDING
-->
${COULD_NOT_BE_REACHED_NOTICE} The last thing heard from it was its word that it was busy running a command and could not hear this session, so Claude on ${REMOTE_MACHINE_NAME} and the computer are most likely fine and it is the connection between them and this session that is down: ask the user to check that computer's network, and not to quit Claude there, which would stop the command it is running${IS_RETURN_NOTED?"":"; and to say when it is back"}. Do not call ${REMOTE_MACHINE_NAME} again ${AWAY_UNTIL_CONDITION}: do the rest of the task without ${REMOTE_MACHINE_NAME}, and tell the user what is blocked.${RECHECK_ON_REQUEST_ENDING}
