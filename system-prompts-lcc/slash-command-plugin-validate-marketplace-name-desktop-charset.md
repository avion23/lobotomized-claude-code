<!--
name: '/plugin validate: marketplace name Desktop charset warning'
description: >-
  Warning that a marketplace name is not accepted by Claude Desktop's charset
  rules, so Desktop's managed marketplace sync will reject it.
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_MARKETPLACE_NAME_DESKTOP_CHARSET_VAR_0
-->
Marketplace name "${SLASH_COMMAND_PLUGIN_VALIDATE_MARKETPLACE_NAME_DESKTOP_CHARSET_VAR_0.name}" is not accepted by Claude Desktop (letters, digits, ".", "_", "-"; must start alphanumeric; max 128 chars). 
