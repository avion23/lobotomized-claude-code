<!--
name: '/plugin install: plugin manifest read failed'
description: >-
  Install failure when the fetched plugin's .claude-plugin manifest file exists
  but cannot be read; thrown by the manifest loader while caching the plugin.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_READ_FAILED_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_READ_FAILED_VAR_1
  - SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_READ_FAILED_VAR_2
-->
Plugin ${SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_READ_FAILED_VAR_0}: failed to read manifest file at ${SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_READ_FAILED_VAR_1}.

Read error: ${SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_READ_FAILED_VAR_2}
