<!--
name: CronCreate durable parameter
description: >-
  input_schema param description for the CronCreate tool's durable field;
  serialized into the model's tool list, so model-facing.
ccVersion: 2.1.191
-->
true = persist to .claude/scheduled_tasks.json and survive restarts. false (default) = in-memory only, dies when this Claude session ends. Use true only when the user asks the task to survive across sessions.
