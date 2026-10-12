<!--
name: '/plugin install: plugin cache version folder refused by storage layer'
description: >-
  Install failure when the storage layer refuses to empty a plugin's cache
  version folder, so nothing was removed.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_CACHE_VERSION_FOLDER_REFUSED_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_CACHE_VERSION_FOLDER_REFUSED_VAR_1
  - SLASH_COMMAND_PLUGIN_INSTALL_CACHE_VERSION_FOLDER_REFUSED_VAR_2
-->
Could not empty ${SLASH_COMMAND_PLUGIN_INSTALL_CACHE_VERSION_FOLDER_REFUSED_VAR_0}: the storage layer refused the version folder (${SLASH_COMMAND_PLUGIN_INSTALL_CACHE_VERSION_FOLDER_REFUSED_VAR_1(SLASH_COMMAND_PLUGIN_INSTALL_CACHE_VERSION_FOLDER_REFUSED_VAR_2.error)}); check that plugin cache folder — nothing was removed — and then retry the install or the update.
