<!--
name: 'Slash Command: marketplace clone failed'
description: >-
  /plugin marketplace add/update error when cloning the marketplace repository
  fails, quoting git stderr.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_FAILED_VAR_0
-->
Failed to clone marketplace repository: ${SLASH_COMMAND_PLUGIN_MARKETPLACE_CLONE_FAILED_VAR_0.stderr}
