<!--
name: 'Plugin validate: derived name not kebab'
description: 'Finding: the folder-derived name is not kebab-case.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_DERIVED_NAME_NOT_KEBAB_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_DERIVED_NAME_NOT_KEBAB_VAR_1
-->
There is no plugin.json, so ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_DERIVED_NAME_NOT_KEBAB_VAR_0(SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_DERIVED_NAME_NOT_KEBAB_VAR_1)} stands in for the plugin name, and it is not kebab-case. Claude Code accepts it, but the Claude.ai marketplace sync requires kebab-case (lowercase letters, digits, and hyphens only, e.g., "my-plugin").
