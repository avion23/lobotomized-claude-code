<!--
name: '/plugin install: installed_plugins.json backup could not be written'
description: >-
  Install failure when installed_plugins.json is unreadable and the side copy
  kept before rebuilding it cannot be written.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_BACKUP_WRITE_FAILED_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_BACKUP_WRITE_FAILED_VAR_1
-->
installed_plugins.json cannot be read, and it was not changed. Before it is rebuilt, its contents are kept in a file beside it, but that file (${SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_BACKUP_WRITE_FAILED_VAR_0}) could not be written: ${SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_BACKUP_WRITE_FAILED_VAR_1}. Free disk space or make the plugins folder writable, or move installed_plugins.json aside by hand, then try again.
