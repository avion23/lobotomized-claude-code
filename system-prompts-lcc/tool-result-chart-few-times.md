<!--
name: 'Chart Tool: Too Few Times'
description: Chart refusal when a time column has too few distinct times to infer the axis.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_CHART_FEW_TIMES_VAR_0
  - TOOL_RESULT_CHART_FEW_TIMES_VAR_1
  - TOOL_RESULT_CHART_FEW_TIMES_VAR_2
  - TOOL_RESULT_CHART_FEW_TIMES_VAR_3
-->
${TOOL_RESULT_CHART_FEW_TIMES_VAR_0.name} holds ${TOOL_RESULT_CHART_FEW_TIMES_VAR_1(TOOL_RESULT_CHART_FEW_TIMES_VAR_2,"time")}, too few to find the time axis unasked (that takes ${TOOL_RESULT_CHART_FEW_TIMES_VAR_3}). Name x and y
