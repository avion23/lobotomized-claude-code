<!--
name: 'System Reminder: Attached machine could not be reached'
description: >-
  Opens the notice that an attached machine could not be reached, with when it
  was last heard from and the reason, and that the call did not run
ccVersion: 2.1.304
variables:
  - REMOTE_MACHINE_NAME
  - LAST_HEARD_FROM_CLAUSE
  - UNREACHABLE_REASON
-->
${REMOTE_MACHINE_NAME} could not be reached from this session (${LAST_HEARD_FROM_CLAUSE}${UNREACHABLE_REASON}); the call did not run.
