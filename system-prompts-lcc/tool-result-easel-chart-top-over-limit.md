<!--
name: 'Tool result: easel chart top over limit'
description: Note that a requested top N exceeds what one chart can draw.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_EASEL_CHART_TOP_OVER_LIMIT_VAR_0
  - TOOL_RESULT_EASEL_CHART_TOP_OVER_LIMIT_VAR_1
-->
top ${TOOL_RESULT_EASEL_CHART_TOP_OVER_LIMIT_VAR_0.top}: a chart draws at most ${TOOL_RESULT_EASEL_CHART_TOP_OVER_LIMIT_VAR_1(TOOL_RESULT_EASEL_CHART_TOP_OVER_LIMIT_VAR_0.form,TOOL_RESULT_EASEL_CHART_TOP_OVER_LIMIT_VAR_0.formLimit)}
