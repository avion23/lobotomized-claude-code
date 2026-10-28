<!--
name: 'Tool Result: Windows short name may open adopt.json'
description: >-
  Refusal message when a file name has the shape of a Windows 8.3 short name
  that may open adopt.json in the config directory
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_WINDOWS_SHORT_NAME_ADOPT_JSON_REFUSAL_VAR_0
-->
This file name has the shape of a Windows short name (such as ADOPT~1.JSO), which may open adopt.json. ${TOOL_RESULT_WINDOWS_SHORT_NAME_ADOPT_JSON_REFUSAL_VAR_0.message}. A name with no "~" followed by a digit is not refused for this reason.
