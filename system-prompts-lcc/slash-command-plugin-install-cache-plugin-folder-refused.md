<!--
name: '/plugin install: plugin cache folder refused by storage layer'
description: >-
  Install failure when the storage layer refuses to prepare a plugin's cache
  folder (ELOOP), so the plugin version was not cached.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_CACHE_PLUGIN_FOLDER_REFUSED_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_CACHE_PLUGIN_FOLDER_REFUSED_VAR_1
  - SLASH_COMMAND_PLUGIN_INSTALL_CACHE_PLUGIN_FOLDER_REFUSED_VAR_2
-->
Could not prepare the plugin cache folder of ${SLASH_COMMAND_PLUGIN_INSTALL_CACHE_PLUGIN_FOLDER_REFUSED_VAR_0}: the storage layer refused it (${SLASH_COMMAND_PLUGIN_INSTALL_CACHE_PLUGIN_FOLDER_REFUSED_VAR_1(SLASH_COMMAND_PLUGIN_INSTALL_CACHE_PLUGIN_FOLDER_REFUSED_VAR_2.error)}); check that plugin cache folder — the plugin version was not cached — and then retry the install or the update.
