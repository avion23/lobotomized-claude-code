<!--
name: '/plugin marketplace: existing directory could not be moved aside'
description: >-
  Marketplace refresh failure when the existing marketplace directory cannot be
  moved aside before the new clone replaces it.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_MOVE_ASIDE_FAILED_VAR_0
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_MOVE_ASIDE_FAILED_VAR_1
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_MOVE_ASIDE_FAILED_VAR_2
-->
Failed to move the existing marketplace directory aside. Please manually delete the directory at ${SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_MOVE_ASIDE_FAILED_VAR_0} and try again.

Technical details: ${SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_MOVE_ASIDE_FAILED_VAR_1(SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_MOVE_ASIDE_FAILED_VAR_2)}
