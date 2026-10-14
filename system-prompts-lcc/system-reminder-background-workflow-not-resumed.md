<!--
name: Background workflow not-resumed notice
description: >-
  Task-notification injected to the model that a checkpointed workflow was not
  resumed, with resume steps.
ccVersion: 2.1.300
variables:
  - SYSTEM_REMINDER_BACKGROUND_WORKFLOW_NOT_RESUMED_VAR_0
  - SYSTEM_REMINDER_BACKGROUND_WORKFLOW_NOT_RESUMED_VAR_1
  - SYSTEM_REMINDER_BACKGROUND_WORKFLOW_NOT_RESUMED_VAR_2
-->
Background workflow "${SYSTEM_REMINDER_BACKGROUND_WORKFLOW_NOT_RESUMED_VAR_0(SYSTEM_REMINDER_BACKGROUND_WORKFLOW_NOT_RESUMED_VAR_1.description)}" was checkpointed for the background fork but the fork failed to spawn; it was not resumed.${SYSTEM_REMINDER_BACKGROUND_WORKFLOW_NOT_RESUMED_VAR_2}
