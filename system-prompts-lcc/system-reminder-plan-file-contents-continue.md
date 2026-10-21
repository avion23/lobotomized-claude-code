<!--
name: 'System Reminder: plan contents and continue'
description: >-
  plan_file_reference body with plan contents and the instruction to continue if
  relevant
ccVersion: 2.1.301
variables:
  - SYSTEM_REMINDER_PLAN_FILE_CONTENTS_CONTINUE_VAR_0
-->
${SYSTEM_REMINDER_PLAN_FILE_CONTENTS_CONTINUE_VAR_0.planFilePath?`A plan file exists from plan mode at: ${SYSTEM_REMINDER_PLAN_FILE_CONTENTS_CONTINUE_VAR_0.planFilePath}`:"A plan exists from plan mode."}

Plan contents:

${SYSTEM_REMINDER_PLAN_FILE_CONTENTS_CONTINUE_VAR_0.planContent}

If this plan is relevant to the current work and not already complete, continue working on it.
