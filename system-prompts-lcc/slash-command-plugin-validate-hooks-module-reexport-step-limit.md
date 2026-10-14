<!--
name: 'Slash Command: Plugin validate hooks module re-export step limit'
description: >-
  Refuses re-export chains that take more steps than a scan allows and suggests
  fewer export * statements
ccVersion: 2.1.299
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MODULE_REEXPORT_STEP_LIMIT_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MODULE_REEXPORT_STEP_LIMIT_VAR_1
-->
the re-exports of "${SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MODULE_REEXPORT_STEP_LIMIT_VAR_0.pluginName}" took ${SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MODULE_REEXPORT_STEP_LIMIT_VAR_0.exportSteps.taken} steps to follow, more than the ${SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MODULE_REEXPORT_STEP_LIMIT_VAR_1} a scan allows: write fewer \`export *\`, or import each name from the file that declares it
