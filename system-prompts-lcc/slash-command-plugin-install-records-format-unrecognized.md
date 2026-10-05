<!--
name: Plugin install — installed_plugins.json format not recognized
description: >-
  Explanatory clause for why a plugin operation failed: the local
  installed_plugins.json is in a format this build doesn't recognize (a newer
  build wrote it), so plugins cannot be changed and some may not load; tells the
  user to update Claude Code or use the version that wrote the file.
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_FORMAT_UNRECOGNIZED_VAR_0
  - SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_FORMAT_UNRECOGNIZED_VAR_1
-->
installed_plugins.json is in a format (version ${SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_FORMAT_UNRECOGNIZED_VAR_0.formatVersion??"unknown"}) that this version of Claude Code does not know, so plugins cannot be changed from this version, and some may not load. Update Claude Code on this machine (claude update), or change plugins with the version of Claude Code that wrote ${SLASH_COMMAND_PLUGIN_INSTALL_RECORDS_FORMAT_UNRECOGNIZED_VAR_1()}.
