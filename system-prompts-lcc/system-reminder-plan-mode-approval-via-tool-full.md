<!--
name: 'System Reminder: Plan mode approval via tool (full)'
description: >-
  Plan mode instruction to pass the whole final plan to the plan-approval tool,
  how approval and decline work, and that the turn should only end with a
  clarifying question or that tool
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_PLAN_MODE_APPROVAL_VIA_TOOL_FULL_VAR_0
  - SYSTEM_REMINDER_PLAN_MODE_APPROVAL_VIA_TOOL_FULL_VAR_1
-->
When your plan is final, call ${SYSTEM_REMINDER_PLAN_MODE_APPROVAL_VIA_TOOL_FULL_VAR_0} with the whole plan as its \`plan\` argument. The user sees it on an approval card: if they approve, plan mode ends; if they decline, you stay in plan mode and revise the plan. Your turn should only end with ${SYSTEM_REMINDER_PLAN_MODE_APPROVAL_VIA_TOOL_FULL_VAR_1} (to clarify requirements or choose between approaches) or ${SYSTEM_REMINDER_PLAN_MODE_APPROVAL_VIA_TOOL_FULL_VAR_0} (to request plan approval). Do NOT ask about plan approval in any other way.
