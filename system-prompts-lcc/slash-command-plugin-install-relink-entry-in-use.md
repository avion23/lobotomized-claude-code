<!--
name: '/plugin install: cache path entry in use during relink'
description: >-
  Install failure when another session is recorded as using the entry at the
  plugin's cache path, so the link farm could not be relinked.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_RELINK_ENTRY_IN_USE_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_RELINK_ENTRY_IN_USE_VAR_1
-->
Could not link ${SLASH_COMMAND_PLUGIN_INSTALL_RELINK_ENTRY_IN_USE_VAR_0} ${SLASH_COMMAND_PLUGIN_INSTALL_RELINK_ENTRY_IN_USE_VAR_1}: another session is recorded as using the entry at its cache path; retry the load or the install.
