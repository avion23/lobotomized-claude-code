<!--
name: '/plugin install: plugin directory is not a directory'
description: >-
  Install failure when the plugin's marketplace or plugin folder in the cache is
  a dangling link or a file instead of a directory.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_PLUGIN_DIR_NOT_DIRECTORY_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_PLUGIN_DIR_NOT_DIRECTORY_VAR_1
  - SLASH_COMMAND_PLUGIN_INSTALL_PLUGIN_DIR_NOT_DIRECTORY_VAR_2
-->
Could not ${SLASH_COMMAND_PLUGIN_INSTALL_PLUGIN_DIR_NOT_DIRECTORY_VAR_0} ${SLASH_COMMAND_PLUGIN_INSTALL_PLUGIN_DIR_NOT_DIRECTORY_VAR_1} ${SLASH_COMMAND_PLUGIN_INSTALL_PLUGIN_DIR_NOT_DIRECTORY_VAR_2}: its plugin directory is not a directory (a dangling link, or a file wearing the marketplace or plugin folder name); make it a directory, or retry the install if it was being moved.
