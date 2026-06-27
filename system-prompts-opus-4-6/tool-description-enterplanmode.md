<!--
name: 'Tool Description: EnterPlanMode'
description: >-
  Tool description for entering plan mode to explore and design implementation
  approaches
ccVersion: 2.1.145
variables:
  - ASK_USER_QUESTION_TOOL_NAME
  - CONDITIONAL_WHAT_HAPPENS_NOTE_FN
-->
Use this tool before non-trivial implementation tasks to get user sign-off on your approach. Skip for single-line fixes, trivial edits, or tasks with very specific instructions.

${CONDITIONAL_WHAT_HAPPENS_NOTE_FN()}
