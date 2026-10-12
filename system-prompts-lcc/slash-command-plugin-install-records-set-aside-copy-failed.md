<!--
name: '/plugin install: set-aside install records could not be copied'
description: >-
  Install failure when installed_plugins.json holds unusable records whose
  side-file copy cannot be written, so the file was not changed.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_SET_ASIDE_COPY_FAILED_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_SET_ASIDE_COPY_FAILED_VAR_1
-->
installed_plugins.json was not changed: it holds records under names that no version of Claude Code can use; they are copied to a side file before they are removed, and that copy could not be written to ${SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_SET_ASIDE_COPY_FAILED_VAR_0} (${SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_SET_ASIDE_COPY_FAILED_VAR_1}). Make that path writable, or move what stands there away, and try again.
