<!--
name: Plugin(s) failed to load -- count summary
description: >-
  Fallback guidance for the same skill-load-failure path as the named-plugin
  variant, used when no single named plugin matches -- summarizes how many
  plugins failed to load in the session.
ccVersion: 2.1.284
variables:
  - SYSTEM_REMINDER_PLUGIN_DID_NOT_LOAD_COUNT_SUMMARY_VAR_0
  - SYSTEM_REMINDER_PLUGIN_DID_NOT_LOAD_COUNT_SUMMARY_VAR_1
-->
${SYSTEM_REMINDER_PLUGIN_DID_NOT_LOAD_COUNT_SUMMARY_VAR_0.length===1?`1 plugin did not load in this session (${SYSTEM_REMINDER_PLUGIN_DID_NOT_LOAD_COUNT_SUMMARY_VAR_1}); if this skill belongs to it`:`${SYSTEM_REMINDER_PLUGIN_DID_NOT_LOAD_COUNT_SUMMARY_VAR_0.length} plugins did not load in this session (${SYSTEM_REMINDER_PLUGIN_DID_NOT_LOAD_COUNT_SUMMARY_VAR_1}); if this skill belongs to one of them`}, tell the user its plugin could not be loaded here, not that the skill is not installed.
