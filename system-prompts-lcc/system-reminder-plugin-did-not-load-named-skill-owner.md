<!--
name: Named plugin failed to load (skill invocation)
description: >-
  Guidance surfaced to Claude when a specifically-named plugin failed to load,
  instructing it to tell the user the plugin, not the skill, failed to load.
ccVersion: 2.1.284
variables:
  - SYSTEM_REMINDER_PLUGIN_DID_NOT_LOAD_NAMED_SKILL_OWNER_VAR_0
  - SYSTEM_REMINDER_PLUGIN_DID_NOT_LOAD_NAMED_SKILL_OWNER_VAR_1
-->
The plugin "${SYSTEM_REMINDER_PLUGIN_DID_NOT_LOAD_NAMED_SKILL_OWNER_VAR_0}" did not load in this session (${SYSTEM_REMINDER_PLUGIN_DID_NOT_LOAD_NAMED_SKILL_OWNER_VAR_1.category}): tell the user the plugin could not be loaded here, not that the skill is not installed.
