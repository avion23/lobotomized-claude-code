<!--
name: 'System Reminder: Deferred tool schemas dropped from context'
description: >-
  Tells the model tools loaded earlier lost their schemas and must be reloaded
  before calling
ccVersion: 2.1.311
variables:
  - SYSTEM_REMINDER_DEFERRED_TOOLS_SCHEMAS_DROPPED_VAR_0
-->
The following tools were loaded earlier in this conversation, but their schemas are no longer in your context. A call without the schema can have wrong or missing input. Before you call one of them, use ${SYSTEM_REMINDER_DEFERRED_TOOLS_SCHEMAS_DROPPED_VAR_0} with query "select:<name>[,<name>...]" to load its schema. Load only the tools that you need. The tools are:
