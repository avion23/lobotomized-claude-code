<!--
name: Teammate Not Found Did-You-Mean
description: >-
  Model-facing tool_result suggesting a teammate name correction when
  SendMessage targets a non-existent teammate.
ccVersion: 2.1.195
variables:
  - TOOL_RESULT_TEAMMATE_NOT_FOUND_DID_YOU_MEAN_VAR_0
  - TOOL_RESULT_TEAMMATE_NOT_FOUND_DID_YOU_MEAN_VAR_1
-->
No teammate named '${TOOL_RESULT_TEAMMATE_NOT_FOUND_DID_YOU_MEAN_VAR_0.to}' in team '${TOOL_RESULT_TEAMMATE_NOT_FOUND_DID_YOU_MEAN_VAR_1.teamName}'. Did you mean '${TOOL_RESULT_TEAMMATE_NOT_FOUND_DID_YOU_MEAN_VAR_1.suggestion}'?
