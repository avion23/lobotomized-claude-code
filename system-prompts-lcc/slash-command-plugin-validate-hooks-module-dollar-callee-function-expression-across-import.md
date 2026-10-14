<!--
name: >-
  Slash Command: Plugin validate hooks module $ callee function expression
  across import
description: >-
  Refuses following $ across an import into a function expression; only function
  declarations are followed
ccVersion: 2.1.299
variables:
  - >-
    SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MODULE_DOLLAR_CALLEE_FUNCTION_EXPRESSION_ACROSS_IMPORT_VAR_0
-->
$ is passed to "${SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MODULE_DOLLAR_CALLEE_FUNCTION_EXPRESSION_ACROSS_IMPORT_VAR_0.name}", a name bound to a function expression, outside the hook's own file: past an import $ is followed only into a function declaration (function ${SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MODULE_DOLLAR_CALLEE_FUNCTION_EXPRESSION_ACROSS_IMPORT_VAR_0.name}($) { ... }), which a bundle of the module keeps as written
