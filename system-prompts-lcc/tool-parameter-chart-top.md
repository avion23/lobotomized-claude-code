<!--
name: 'Chart Tool Parameter: top'
description: >-
  Chart tool input schema description for top (how many series/bars to draw, per
  form).
ccVersion: 2.1.302
variables:
  - TOOL_PARAMETER_CHART_TOP_VAR_0
  - TOOL_PARAMETER_CHART_TOP_VAR_1
-->
how many to draw: ${TOOL_PARAMETER_CHART_TOP_VAR_0.bars.defaultCount} bars if left out and ${TOOL_PARAMETER_CHART_TOP_VAR_0.bars.maxCount} at most, ${TOOL_PARAMETER_CHART_TOP_VAR_0.line.maxCount} lines at most, ${TOOL_PARAMETER_CHART_TOP_VAR_0.sparks.defaultCount} sparks and ${TOOL_PARAMETER_CHART_TOP_VAR_0.sparks.maxCount} at most, ${TOOL_PARAMETER_CHART_TOP_VAR_0.share.maxCount} parts of a share beside one for the rest, ${TOOL_PARAMETER_CHART_TOP_VAR_0.columns.maxCount} series of columns where they stack, else ${TOOL_PARAMETER_CHART_TOP_VAR_1}. The largest are kept, largest first, and the rest are counted
