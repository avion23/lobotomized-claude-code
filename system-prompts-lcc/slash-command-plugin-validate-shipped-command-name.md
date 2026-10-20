<!--
name: 'Slash Command: Plugin validate shipped command name'
description: >-
  Plugin validate finding that a mod registers a command name Claude Code ships,
  which $.command.register refuses
ccVersion: 2.1.304
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_SHIPPED_COMMAND_NAME_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_SHIPPED_COMMAND_NAME_VAR_1
-->
"/${SLASH_COMMAND_PLUGIN_VALIDATE_SHIPPED_COMMAND_NAME_VAR_0(SLASH_COMMAND_PLUGIN_VALIDATE_SHIPPED_COMMAND_NAME_VAR_1,200)}" is a name Claude Code ships: $.command.register refuses it and the hook that calls it is skipped
