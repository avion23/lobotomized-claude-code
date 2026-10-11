<!--
name: '/plugin install: stray link at cache path during publish'
description: >-
  Install failure when a link sitting at the plugin's cache path cannot be
  removed while the staged copy is published.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_PUBLISH_STRAY_LINK_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_PUBLISH_STRAY_LINK_VAR_1
-->
Could not publish ${SLASH_COMMAND_PLUGIN_INSTALL_PUBLISH_STRAY_LINK_VAR_0} ${SLASH_COMMAND_PLUGIN_INSTALL_PUBLISH_STRAY_LINK_VAR_1}: a link sits at its cache path and could not be removed; remove that link from the plugin cache, then retry the install.
