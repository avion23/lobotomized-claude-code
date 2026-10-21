<!--
name: 'Tool Description: Poll no pending events caveat'
description: >-
  Explains that the no-pending-events answer does not mean nothing is queued for
  the end of the turn
ccVersion: 2.1.301
variables:
  - TOOL_DESCRIPTION_POLL_NO_PENDING_EVENTS_CAVEAT_VAR_0
-->
"${TOOL_DESCRIPTION_POLL_NO_PENDING_EVENTS_CAVEAT_VAR_0}" means only that this call delivered no event. Something may still be queued that this tool never delivers, for example a scheduled prompt or a message held for the end of your turn: it reaches you only after you end your turn.
