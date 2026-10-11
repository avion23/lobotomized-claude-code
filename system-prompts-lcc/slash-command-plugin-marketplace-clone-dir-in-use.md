<!--
name: '/plugin marketplace: existing marketplace directory in use'
description: >-
  Marketplace refresh failure when the existing marketplace directory cannot be
  replaced because it is in use (EBUSY/EPERM/EACCES); the existing copy is kept.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_DIR_IN_USE_VAR_0
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_DIR_IN_USE_VAR_1
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_DIR_IN_USE_VAR_2
-->
Could not replace the marketplace directory at ${SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_DIR_IN_USE_VAR_0} because it is in use; the existing copy was kept and the next refresh will try again.

Technical details: ${SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_DIR_IN_USE_VAR_1(SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_DIR_IN_USE_VAR_2)}
