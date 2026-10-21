<!--
name: 'Plugin validate: could not list folders'
description: 'Note: some folders could not be listed for system files.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_COULD_NOT_LIST_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_COULD_NOT_LIST_VAR_1
-->
Could not list ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_COULD_NOT_LIST_VAR_0(SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_COULD_NOT_LIST_VAR_1)} inside the plugin, so what is under ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_COULD_NOT_LIST_VAR_1.length===1?"it":"them"} was not searched for macOS and Windows system files. Check that ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_COULD_NOT_LIST_VAR_1.length===1?"the folder":"each folder"} can be read, and validate again.
