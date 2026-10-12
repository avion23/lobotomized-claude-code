<!--
name: '/plugin install: plugin manifest is not valid JSON'
description: >-
  Install failure when the fetched plugin's .claude-plugin manifest file exists
  but is not valid JSON; thrown by the manifest loader while caching the plugin.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_JSON_INVALID_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_JSON_INVALID_VAR_1
  - SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_JSON_INVALID_VAR_2
-->
Plugin ${SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_JSON_INVALID_VAR_0} has a corrupt manifest file at ${SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_JSON_INVALID_VAR_1}.

JSON parse error: ${SLASH_COMMAND_PLUGIN_INSTALL_MANIFEST_JSON_INVALID_VAR_2}
