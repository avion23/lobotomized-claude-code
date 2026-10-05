<!--
name: computer_batch action_summary — required for these actions
description: >-
  Tool-schema description text listing which computer/form_input actions must
  carry an action_summary field, appended to the computer_batch/app_batch item
  input description.
ccVersion: 2.1.284
variables:
  - TOOL_DESCRIPTION_COMPUTER_BATCH_ACTION_SUMMARY_REQUIRED_ACTIONS_VAR_0
-->
For computer items whose action is left_click, right_click, double_click, triple_click, left_click_drag, key or type, and for form_input items, include ${TOOL_DESCRIPTION_COMPUTER_BATCH_ACTION_SUMMARY_REQUIRED_ACTIONS_VAR_0} in the item's input, as you would when calling that tool directly.
