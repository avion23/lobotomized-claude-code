<!--
name: Computer screenshot other monitors
description: >-
  Other-monitor list appended to a first screenshot or a changed-monitor
  screenshot.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_COMPUTER_OTHER_ATTACHED_MONITORS_VAR_0
  - TOOL_RESULT_COMPUTER_OTHER_ATTACHED_MONITORS_VAR_1
-->
 Other attached monitors: ${TOOL_RESULT_COMPUTER_OTHER_ATTACHED_MONITORS_VAR_0.map((TOOL_RESULT_COMPUTER_OTHER_ATTACHED_MONITORS_VAR_1)=>`"${TOOL_RESULT_COMPUTER_OTHER_ATTACHED_MONITORS_VAR_1}"`).join(", ")}.
