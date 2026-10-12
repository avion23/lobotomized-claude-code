<!--
name: 'Plugin install folder held: shared-folder notice with admin suffix'
description: >-
  Plugin-folder-held refusal sentence, with ' Ask your administrator.' appended
  when an organization-managed install holds the folder.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_FOLDER_HELD_ASK_ADMINISTRATOR_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_FOLDER_HELD_ASK_ADMINISTRATOR_VAR_1
-->
${SLASH_COMMAND_PLUGIN_INSTALL_FOLDER_HELD_ASK_ADMINISTRATOR_VAR_0}${SLASH_COMMAND_PLUGIN_INSTALL_FOLDER_HELD_ASK_ADMINISTRATOR_VAR_1>0?" Ask your administrator.":""}
