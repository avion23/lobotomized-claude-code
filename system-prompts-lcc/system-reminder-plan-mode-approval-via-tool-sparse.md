<!--
name: 'System Reminder: Plan mode approval via tool (sparse)'
description: >-
  Short plan mode reminder to pass the final plan to the plan-approval tool and
  never ask about approval via text
ccVersion: 2.1.304
variables:
  - SYSTEM_REMINDER_PLAN_MODE_APPROVAL_VIA_TOOL_SPARSE_VAR_0
  - SYSTEM_REMINDER_PLAN_MODE_APPROVAL_VIA_TOOL_SPARSE_VAR_1
-->
When the plan is final, call ${SYSTEM_REMINDER_PLAN_MODE_APPROVAL_VIA_TOOL_SPARSE_VAR_0} with it as \`plan\`. Never ask about plan approval via text or ${SYSTEM_REMINDER_PLAN_MODE_APPROVAL_VIA_TOOL_SPARSE_VAR_1}.
