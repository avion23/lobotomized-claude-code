<!--
name: 'Slash command: plugin hooks file duplicate'
description: >-
  Plugin hook-load error for a manifest.hooks list naming the same file twice;
  for a managed plugin it becomes the 'hooks unknown' cause that blocks a /model
  switch, whose system-display output reaches the model.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_HOOKS_FILE_DUPLICATE_VAR_0
  - SLASH_COMMAND_PLUGIN_HOOKS_FILE_DUPLICATE_VAR_1
-->
Duplicate hooks file detected: ${SLASH_COMMAND_PLUGIN_HOOKS_FILE_DUPLICATE_VAR_0} resolves to already-loaded file ${SLASH_COMMAND_PLUGIN_HOOKS_FILE_DUPLICATE_VAR_1}; manifest.hooks lists it more than once.
