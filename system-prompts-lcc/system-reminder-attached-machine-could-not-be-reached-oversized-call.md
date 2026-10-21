<!--
name: 'System Reminder: Attached machine could not be reached (oversized call)'
description: >-
  Follows the could-not-be-reached notice on this session's side, asking the
  user to check the machine and noting an oversized call won't succeed on retry
ccVersion: 2.1.304
variables:
  - COULD_NOT_BE_REACHED_NOTICE
  - REMOTE_MACHINE_NAME
-->
${COULD_NOT_BE_REACHED_NOTICE} If Claude is not running on ${REMOTE_MACHINE_NAME}, or is no longer connected to this session, ask the user to check it; a call that was too large to deliver will not succeed on a retry.
