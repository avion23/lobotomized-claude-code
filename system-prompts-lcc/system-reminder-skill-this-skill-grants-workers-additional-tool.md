<!--
name: Invoked-skill extra worker permissions
description: >-
  Invoked-skill extra worker permissions. Emitted by the concrete model-context
  route documented below.
ccVersion: 2.1.296
variables:
  - SYSTEM_REMINDER_SKILL_THIS_SKILL_GRANTS_WORKERS_ADDITIONAL_TOOL_VAR_0
  - SYSTEM_REMINDER_SKILL_THIS_SKILL_GRANTS_WORKERS_ADDITIONAL_TOOL_VAR_1
-->
This skill grants workers additional tool permissions: ${SYSTEM_REMINDER_SKILL_THIS_SKILL_GRANTS_WORKERS_ADDITIONAL_TOOL_VAR_0.map(SYSTEM_REMINDER_SKILL_THIS_SKILL_GRANTS_WORKERS_ADDITIONAL_TOOL_VAR_1).join(", ")}
