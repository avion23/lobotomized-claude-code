<!--
name: 'Background result: terminated at turn end'
description: 'ain(e) output, same confirmed Fmo() background-task status consumer.'
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_BASH_BACKGROUND_TERMINATES_WITH_TURN_VAR_0
  - TOOL_RESULT_BASH_BACKGROUND_TERMINATES_WITH_TURN_VAR_1
-->
Its result reaches you only if it finishes while you are still working: it is terminated ${TOOL_RESULT_BASH_BACKGROUND_TERMINATES_WITH_TURN_VAR_0==="final_response"?"when you give your final response":"when your turn ends, since this session takes no further input"}, and nothing can follow that. ${TOOL_RESULT_BASH_BACKGROUND_TERMINATES_WITH_TURN_VAR_1()}
