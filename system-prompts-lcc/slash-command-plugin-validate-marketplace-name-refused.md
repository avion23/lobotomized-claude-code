<!--
name: '/plugin validate: marketplace name refused'
description: >-
  Validation error when a marketplace's declared name is refused (not
  kebab-case/allowed form) and cannot be used to install plugins.
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_MARKETPLACE_NAME_REFUSED_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_MARKETPLACE_NAME_REFUSED_VAR_1
  - SLASH_COMMAND_PLUGIN_VALIDATE_MARKETPLACE_NAME_REFUSED_VAR_2
-->
Claude Code cannot install plugins from marketplace "${SLASH_COMMAND_PLUGIN_VALIDATE_MARKETPLACE_NAME_REFUSED_VAR_0(SLASH_COMMAND_PLUGIN_VALIDATE_MARKETPLACE_NAME_REFUSED_VAR_1.name,64)}". ${SLASH_COMMAND_PLUGIN_VALIDATE_MARKETPLACE_NAME_REFUSED_VAR_2} Change the marketplace's "name".
