<!--
name: 'Slash Command: Plugin install invalid id halves reason'
description: >-
  Explains why a plugin id cannot be installed: each half of plugin@marketplace
  must start with a letter or digit and use only letters, digits, '-', '.' and
  '_', naming which half fails and who can rename it
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_HALVES_REASON_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_HALVES_REASON_VAR_1
-->
Each part of a plugin id (plugin@marketplace) may use only the letters a-z and A-Z, digits, ".", "_" and "-", and must start with a letter or digit. Here ${SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_HALVES_REASON_VAR_0&&!SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_HALVES_REASON_VAR_1?"the marketplace's name does not":!SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_HALVES_REASON_VAR_0&&SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_HALVES_REASON_VAR_1?"the plugin's name does not":"they do not"}; the marketplace's maintainer can rename ${SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_HALVES_REASON_VAR_0||SLASH_COMMAND_PLUGIN_INSTALL_INVALID_ID_HALVES_REASON_VAR_1?"it":"both"}.
