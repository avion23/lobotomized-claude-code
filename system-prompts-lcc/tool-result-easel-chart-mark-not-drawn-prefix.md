<!--
name: 'Tool result: easel chart mark not drawn prefix'
description: >-
  Prefix naming a chart mark (label and time) that was not drawn, followed by
  the reason.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_EASEL_CHART_MARK_NOT_DRAWN_PREFIX_VAR_0
  - TOOL_RESULT_EASEL_CHART_MARK_NOT_DRAWN_PREFIX_VAR_1
-->
${TOOL_RESULT_EASEL_CHART_MARK_NOT_DRAWN_PREFIX_VAR_0===""?"mark":`mark ${TOOL_RESULT_EASEL_CHART_MARK_NOT_DRAWN_PREFIX_VAR_0}`} at ${TOOL_RESULT_EASEL_CHART_MARK_NOT_DRAWN_PREFIX_VAR_1.mark.at} not drawn:
