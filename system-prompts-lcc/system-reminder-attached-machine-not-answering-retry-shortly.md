<!--
name: 'System Reminder: Attached machine not answering (retry shortly)'
description: >-
  Follows the not-answering notice on this session's side, advising to retry
  shortly or ask the user to check Claude is open there
ccVersion: 2.1.304
variables:
  - NOT_ANSWERING_NOTICE
  - REMOTE_MACHINE_NAME
-->
${NOT_ANSWERING_NOTICE} Try again shortly, or ask the user to check that Claude is open on ${REMOTE_MACHINE_NAME}.
