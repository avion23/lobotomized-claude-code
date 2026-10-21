<!--
name: 'Plugin validate: icon path traversal'
description: 'Finding: the icon path contains ''..''.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_ICON_PATH_TRAVERSAL_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_ICON_PATH_TRAVERSAL_VAR_1
-->
Path contains ".." which could be a path traversal attempt: ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_ICON_PATH_TRAVERSAL_VAR_0(SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_ICON_PATH_TRAVERSAL_VAR_1,200)}
