<!--
name: Computer closest menu-title suggestion
description: Optional closest-title suggestion appended to a missing menu-item result.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_COMPUTER_CLOSEST_MATCH_VAR_0
  - TOOL_RESULT_COMPUTER_CLOSEST_MATCH_VAR_1
  - TOOL_RESULT_COMPUTER_CLOSEST_MATCH_VAR_2
-->
 Closest match: ${TOOL_RESULT_COMPUTER_CLOSEST_MATCH_VAR_0.stringify(TOOL_RESULT_COMPUTER_CLOSEST_MATCH_VAR_1(TOOL_RESULT_COMPUTER_CLOSEST_MATCH_VAR_2.closestMatch)??"(title withheld)")}.
