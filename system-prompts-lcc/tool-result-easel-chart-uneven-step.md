<!--
name: 'Tool result: easel chart uneven time step'
description: >-
  easel chart refusal when column timestamps have no even step, telling the
  model to pass one row per period, draw a line, or pass zone local.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_EASEL_CHART_UNEVEN_STEP_VAR_0
-->
the times of ${TOOL_RESULT_EASEL_CHART_UNEVEN_STEP_VAR_0.x} keep no even step (that takes two or more, with few gaps), so a column cannot stand for a period. Rows are not put in buckets of time: pass one row for each period, or draw a line, or pass zone: "local" if the periods are local days
