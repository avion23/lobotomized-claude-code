<!--
name: 'Tool Result: chart field must be one of types'
description: Chart tool input validation error listing the allowed types of an anyOf field.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_CHART_MUST_BE_ANY_OF_TYPES_VAR_0
  - TOOL_RESULT_CHART_MUST_BE_ANY_OF_TYPES_VAR_1
  - TOOL_RESULT_CHART_MUST_BE_ANY_OF_TYPES_VAR_2
-->
${TOOL_RESULT_CHART_MUST_BE_ANY_OF_TYPES_VAR_0} must be ${TOOL_RESULT_CHART_MUST_BE_ANY_OF_TYPES_VAR_1.map((TOOL_RESULT_CHART_MUST_BE_ANY_OF_TYPES_VAR_2)=>TOOL_RESULT_CHART_MUST_BE_ANY_OF_TYPES_VAR_2.type).join(" or ")}
