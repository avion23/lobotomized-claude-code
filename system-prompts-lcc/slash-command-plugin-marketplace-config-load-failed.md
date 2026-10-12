<!--
name: 'Slash Command: marketplace config load failed'
description: >-
  /plugin marketplace error when reading the known-marketplaces configuration
  through the storage backend fails.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_CONFIG_LOAD_FAILED_VAR_0
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_CONFIG_LOAD_FAILED_VAR_1
-->
Failed to load marketplace configuration: ${SLASH_COMMAND_PLUGIN_MARKETPLACE_CONFIG_LOAD_FAILED_VAR_0(SLASH_COMMAND_PLUGIN_MARKETPLACE_CONFIG_LOAD_FAILED_VAR_1.error)}
