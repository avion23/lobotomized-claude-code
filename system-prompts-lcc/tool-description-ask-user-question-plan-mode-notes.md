<!--
name: 'Tool Description: AskUserQuestion plan mode notes'
description: >-
  AskUserQuestion prompt notes on plan mode: switch with the plan tool, do not
  ask whether the plan is ready
ccVersion: 2.1.301
variables:
  - TOOL_DESCRIPTION_ASK_USER_QUESTION_PLAN_MODE_NOTES_VAR_0
  - TOOL_DESCRIPTION_ASK_USER_QUESTION_PLAN_MODE_NOTES_VAR_1
  - TOOL_DESCRIPTION_ASK_USER_QUESTION_PLAN_MODE_NOTES_VAR_2
-->
${TOOL_DESCRIPTION_ASK_USER_QUESTION_PLAN_MODE_NOTES_VAR_0}
Some notes about plan mode, which is different from asking the user a simple question:
To switch into plan mode, use ${TOOL_DESCRIPTION_ASK_USER_QUESTION_PLAN_MODE_NOTES_VAR_1} (not this tool). Once in plan mode, use this tool to clarify requirements or choose between approaches BEFORE finalizing your plan. Do NOT use this tool to ask "Is my plan ready?", "Should I proceed?", or otherwise reference "the plan" in questions — the user cannot see the plan until you call ${TOOL_DESCRIPTION_ASK_USER_QUESTION_PLAN_MODE_NOTES_VAR_2} for approval.
