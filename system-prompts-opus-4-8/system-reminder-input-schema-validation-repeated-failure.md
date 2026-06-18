<!--
name: 'System Reminder: Repeated tool-input schema validation failure'
description: >-
  Injected nudge after a tool call fails InputValidationError N times in a row,
  restating the tool's input schema and telling the model to match names/types
  exactly.
ccVersion: 2.1.181
variables:
  - SYSTEM_REMINDER_INPUT_SCHEMA_VALIDATION_REPEATED_FAILURE_VAR_0
  - SYSTEM_REMINDER_INPUT_SCHEMA_VALIDATION_REPEATED_FAILURE_VAR_1
  - SYSTEM_REMINDER_INPUT_SCHEMA_VALIDATION_REPEATED_FAILURE_VAR_2
-->


This call has now failed validation ${SYSTEM_REMINDER_INPUT_SCHEMA_VALIDATION_REPEATED_FAILURE_VAR_0} times in a row. The ${SYSTEM_REMINDER_INPUT_SCHEMA_VALIDATION_REPEATED_FAILURE_VAR_1} tool's input schema is: ${SYSTEM_REMINDER_INPUT_SCHEMA_VALIDATION_REPEATED_FAILURE_VAR_2}. Match the parameter names and types exactly on the next attempt.
