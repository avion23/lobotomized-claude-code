<!--
name: Computer unattended already-granted apps
description: >-
  List of apps that remain available when a scheduled run cannot obtain
  additional grants.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_COMPUTER_ALREADY_GRANTED_APPS_REMAIN_AVAILABLE_VAR_0
  - TOOL_RESULT_COMPUTER_ALREADY_GRANTED_APPS_REMAIN_AVAILABLE_VAR_1
-->
 Already-granted apps remain available: ${TOOL_RESULT_COMPUTER_ALREADY_GRANTED_APPS_REMAIN_AVAILABLE_VAR_0.map((TOOL_RESULT_COMPUTER_ALREADY_GRANTED_APPS_REMAIN_AVAILABLE_VAR_1)=>TOOL_RESULT_COMPUTER_ALREADY_GRANTED_APPS_REMAIN_AVAILABLE_VAR_1.displayName).join(", ")}.
