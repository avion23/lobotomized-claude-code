<!--
name: '/plugin validate: plugin name not kebab-case'
description: >-
  Composite validation error reported when a plugin's declared name is not
  kebab-case, with an interpolated reason clause and marketplace-sync note.
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_NAME_NOT_KEBAB_CASE_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_NAME_NOT_KEBAB_CASE_VAR_1
-->
Plugin name "${SLASH_COMMAND_PLUGIN_VALIDATE_NAME_NOT_KEBAB_CASE_VAR_0.name}" is not kebab-case. ${SLASH_COMMAND_PLUGIN_VALIDATE_NAME_NOT_KEBAB_CASE_VAR_1} Claude.ai marketplace sync requires kebab-case (lowercase letters, digits, and hyphens only, e.g., "my-plugin").
