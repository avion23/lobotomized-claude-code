<!--
name: 'Tool Result: Hook rewrite — tell user to turn off hook'
description: >-
  Tail clause telling Claude to continue other tasks and tell the user auto mode
  could not check the call because a hook or plugin changes it
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_TELL_USER_TURN_OFF_VAR_0
-->
continue with other tasks and tell the user that auto mode could not check this ${TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_TELL_USER_TURN_OFF_VAR_0} call because a hook or plugin changes it, and that they can turn that hook or plugin off (or ask their administrator to) or switch out of auto mode to approve it themselves.
