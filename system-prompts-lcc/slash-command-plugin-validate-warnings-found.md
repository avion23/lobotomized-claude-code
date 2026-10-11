<!--
name: '/plugin validate: warnings found'
description: >-
  Header counting the warnings found in one validated file, before the warning
  list.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_WARNINGS_FOUND_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_WARNINGS_FOUND_VAR_1
  - SLASH_COMMAND_PLUGIN_VALIDATE_WARNINGS_FOUND_VAR_2
-->
${SLASH_COMMAND_PLUGIN_VALIDATE_WARNINGS_FOUND_VAR_0.warning} Found ${SLASH_COMMAND_PLUGIN_VALIDATE_WARNINGS_FOUND_VAR_1.warnings.length} ${SLASH_COMMAND_PLUGIN_VALIDATE_WARNINGS_FOUND_VAR_2(SLASH_COMMAND_PLUGIN_VALIDATE_WARNINGS_FOUND_VAR_1.warnings.length,"warning")}:

