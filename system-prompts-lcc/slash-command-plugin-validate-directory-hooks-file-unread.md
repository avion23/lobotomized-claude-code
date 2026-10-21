<!--
name: 'Plugin validate: hooks file unread'
description: 'Finding: hooks file not read; the directory refuses it.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_HOOKS_FILE_UNREAD_VAR_0
-->
This hooks file is a symlink, goes through one, is not a regular file, or is larger than ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_HOOKS_FILE_UNREAD_VAR_0} bytes, and was not read. The plugin loader reads it anyway and would run these hooks unscreened, so the directory refuses them.
