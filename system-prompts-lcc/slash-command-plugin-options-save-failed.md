<!--
name: /plugin options save failed
description: >-
  Plugin install/configure result when the plugin was installed but its options
  could not be saved, optionally noting the plugin failed to load.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_OPTIONS_SAVE_FAILED_VAR_0
  - SLASH_COMMAND_PLUGIN_OPTIONS_SAVE_FAILED_VAR_1
  - SLASH_COMMAND_PLUGIN_OPTIONS_SAVE_FAILED_VAR_2
-->
${SLASH_COMMAND_PLUGIN_OPTIONS_SAVE_FAILED_VAR_0} but failed to save config: ${SLASH_COMMAND_PLUGIN_OPTIONS_SAVE_FAILED_VAR_1}${SLASH_COMMAND_PLUGIN_OPTIONS_SAVE_FAILED_VAR_2?" The plugin couldn't be loaded — see /plugin for details.":""}
