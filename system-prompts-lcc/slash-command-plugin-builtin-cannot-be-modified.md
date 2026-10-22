<!--
name: 'Slash Command: built-in plugin cannot be installed/updated'
description: 'Plugin operation refusal for a built-in plugin, pointing to enable/disable.'
ccVersion: 2.1.308
variables:
  - SLASH_COMMAND_PLUGIN_BUILTIN_CANNOT_BE_MODIFIED_VAR_0
  - SLASH_COMMAND_PLUGIN_BUILTIN_CANNOT_BE_MODIFIED_VAR_1
  - SLASH_COMMAND_PLUGIN_BUILTIN_CANNOT_BE_MODIFIED_VAR_2
-->
This is a built-in plugin — built-in plugins cannot be installed, updated or uninstalled. ${SLASH_COMMAND_PLUGIN_BUILTIN_CANNOT_BE_MODIFIED_VAR_0(SLASH_COMMAND_PLUGIN_BUILTIN_CANNOT_BE_MODIFIED_VAR_1)?.SLASH_COMMAND_PLUGIN_BUILTIN_CANNOT_BE_MODIFIED_VAR_2??"Use `claude plugin enable` / `claude plugin disable` to turn it on or off."}
