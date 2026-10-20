<!--
name: 'Tool Result: ExitPlanMode plan too large'
description: >-
  Refusal that the plan is too many bytes as JSON for the approval card,
  explaining how characters count, asking to shorten it
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_EXITPLANMODE_PLAN_TOO_LARGE_VAR_0
  - TOOL_RESULT_EXITPLANMODE_PLAN_TOO_LARGE_VAR_1
-->
The plan is ${TOOL_RESULT_EXITPLANMODE_PLAN_TOO_LARGE_VAR_0} bytes as JSON, over the ${TOOL_RESULT_EXITPLANMODE_PLAN_TOO_LARGE_VAR_1} that the user's approval card can carry. A quote, backslash or line break counts as two bytes, and a non-ASCII character as two to four. Shorten the plan and call this tool again.
