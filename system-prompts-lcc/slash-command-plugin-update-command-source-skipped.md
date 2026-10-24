<!--
name: 'Slash Command: plugin update command source skipped'
description: >-
  Update result: plugin installed by running a command is left to per-session
  re-resolve or explicit update.
ccVersion: 2.1.308
variables:
  - SLASH_COMMAND_PLUGIN_UPDATE_COMMAND_SOURCE_SKIPPED_VAR_0
  - SLASH_COMMAND_PLUGIN_UPDATE_COMMAND_SOURCE_SKIPPED_VAR_1
  - SLASH_COMMAND_PLUGIN_UPDATE_COMMAND_SOURCE_SKIPPED_VAR_2
  - SLASH_COMMAND_PLUGIN_UPDATE_COMMAND_SOURCE_SKIPPED_VAR_3
  - SLASH_COMMAND_PLUGIN_UPDATE_COMMAND_SOURCE_SKIPPED_VAR_4
-->
${SLASH_COMMAND_PLUGIN_UPDATE_COMMAND_SOURCE_SKIPPED_VAR_0(SLASH_COMMAND_PLUGIN_UPDATE_COMMAND_SOURCE_SKIPPED_VAR_1,200)} is installed by running a command, which the background marketplace update never runs; it is left to the per-session re-resolve (when that is enabled) or an explicit update — ${SLASH_COMMAND_PLUGIN_UPDATE_COMMAND_SOURCE_SKIPPED_VAR_2("plugin update",SLASH_COMMAND_PLUGIN_UPDATE_COMMAND_SOURCE_SKIPPED_VAR_3,{extra:SLASH_COMMAND_PLUGIN_UPDATE_COMMAND_SOURCE_SKIPPED_VAR_4,fallback:"a per-plugin update reviews it"})}.
