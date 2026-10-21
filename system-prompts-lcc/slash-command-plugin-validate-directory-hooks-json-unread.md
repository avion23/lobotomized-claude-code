<!--
name: 'Plugin validate: hooks.json unread'
description: 'Finding: hooks.json not read; the directory refuses it.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_HOOKS_JSON_UNREAD_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_HOOKS_JSON_UNREAD_VAR_1
-->
${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_HOOKS_JSON_UNREAD_VAR_0} — hooks are read without following symlinks and are capped at ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_HOOKS_JSON_UNREAD_VAR_1} bytes. The plugin loader has neither limit and would run these hooks unscreened, so the directory refuses them.
