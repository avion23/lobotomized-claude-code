<!--
name: 'Plugin validate: files taken from repo root'
description: 'Note: README/license were taken from the repository root.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_TAKEN_FROM_REPO_ROOT_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_TAKEN_FROM_REPO_ROOT_VAR_1
-->
${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_TAKEN_FROM_REPO_ROOT_VAR_0(SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_TAKEN_FROM_REPO_ROOT_VAR_1.used.join(" and "),300)} ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_TAKEN_FROM_REPO_ROOT_VAR_1.used.length===1?"was":"were"} taken from it, because this plugin folder has none of its own.
