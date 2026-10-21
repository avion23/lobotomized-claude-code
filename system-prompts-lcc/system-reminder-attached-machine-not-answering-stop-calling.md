<!--
name: 'System Reminder: Attached machine not answering (stop calling)'
description: >-
  Follows the not-answering notice, barring further calls this turn and telling
  the user what brings the machine back
ccVersion: 2.1.304
variables:
  - NOT_ANSWERING_NOTICE
  - REMOTE_MACHINE_NAME
  - ATTACHED_MACHINE_MESSAGE_REGISTRY
-->
${NOT_ANSWERING_NOTICE} Do not call ${REMOTE_MACHINE_NAME} again in this turn: do the rest of the task without ${REMOTE_MACHINE_NAME}, and tell the user what is blocked and that opening Claude on ${REMOTE_MACHINE_NAME}, with the computer awake and online, is what brings it back. ${ATTACHED_MACHINE_MESSAGE_REGISTRY["away.ending"]()}
