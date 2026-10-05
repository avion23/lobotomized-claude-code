<!--
name: Plugin install — invalid plugin id
description: >-
  Error shown by /plugin install when the plugin's own id fails the plugin-id
  validation rules.
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_VAR_1
  - SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_VAR_2
-->
Plugin "${SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_VAR_0}" cannot be installed, because its id is invalid: ${SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_VAR_1}${SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_VAR_2}
