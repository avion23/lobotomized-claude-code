<!--
name: 'Plugin validate: icon path characters'
description: 'Finding: the icon path has disallowed characters.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_ICON_PATH_CHARACTERS_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_ICON_PATH_CHARACTERS_VAR_1
-->
manifest \`icon\` path ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_ICON_PATH_CHARACTERS_VAR_0(SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_ICON_PATH_CHARACTERS_VAR_1,120)} contains characters that are not allowed in a listing path (quotes, angle brackets, backslash, backtick, whitespace or control characters); it was dropped from the listing preview.
