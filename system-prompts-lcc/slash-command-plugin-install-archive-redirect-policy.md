<!--
name: '/plugin install: archive redirect policy'
description: >-
  Middle fragment of the plugin-archive redirect refusal quoting the archive URL
  policy every hop must satisfy.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_ARCHIVE_REDIRECT_POLICY_VAR_0
-->
every hop must satisfy the archive URL policy (${SLASH_COMMAND_PLUGIN_INSTALL_ARCHIVE_REDIRECT_POLICY_VAR_0.replace(/^Archive URLs must /,"")}): 
