<!--
name: 'Tool Result: Assistant-Mode Blocking Budget Exceeded'
description: >-
  Bash tool_result when a command exceeds the assistant-mode blocking budget and
  is moved to background; advises delegating long-running work.
ccVersion: 2.1.178
variables:
  - TOOL_DESCRIPTION_BASH_ASSISTANT_MODE_BLOCKING_BUDGET_EXCEEDED_VAR_0
  - TOOL_DESCRIPTION_BASH_ASSISTANT_MODE_BLOCKING_BUDGET_EXCEEDED_VAR_1
  - TOOL_DESCRIPTION_BASH_ASSISTANT_MODE_BLOCKING_BUDGET_EXCEEDED_VAR_2
-->
Command exceeded the assistant-mode blocking budget (${TOOL_DESCRIPTION_BASH_ASSISTANT_MODE_BLOCKING_BUDGET_EXCEEDED_VAR_0/1000}s) and was moved to the background with ID: ${TOOL_DESCRIPTION_BASH_ASSISTANT_MODE_BLOCKING_BUDGET_EXCEEDED_VAR_1}. Still running; you will be notified when it completes. Output: ${TOOL_DESCRIPTION_BASH_ASSISTANT_MODE_BLOCKING_BUDGET_EXCEEDED_VAR_2}. In assistant mode, delegate long-running work to a subagent or use run_in_background.
