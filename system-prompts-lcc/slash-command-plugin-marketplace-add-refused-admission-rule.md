<!--
name: 'Slash Command: marketplace add refused by admission rule'
description: >-
  /plugin marketplace add refusal by the registry admission rule before the
  marketplace name is known, with the cause and fix hint.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_ADD_REFUSED_ADMISSION_RULE_VAR_0
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_ADD_REFUSED_ADMISSION_RULE_VAR_1
-->
Cannot add this marketplace: ${SLASH_COMMAND_PLUGIN_MARKETPLACE_ADD_REFUSED_ADMISSION_RULE_VAR_0.cause}; ${SLASH_COMMAND_PLUGIN_MARKETPLACE_ADD_REFUSED_ADMISSION_RULE_VAR_1[SLASH_COMMAND_PLUGIN_MARKETPLACE_ADD_REFUSED_ADMISSION_RULE_VAR_0.kind]}.
