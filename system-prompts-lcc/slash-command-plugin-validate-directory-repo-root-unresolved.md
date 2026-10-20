<!--
name: 'Plugin validate: repo root unresolved'
description: 'Note: stopped looking for a repo root where the real path is unknown.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNRESOLVED_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNRESOLVED_VAR_1
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNRESOLVED_VAR_2
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNRESOLVED_VAR_3
-->
Stopped looking for a repository root at ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNRESOLVED_VAR_0(SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNRESOLVED_VAR_1.dir,SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNRESOLVED_VAR_2)}, because this command could not find where that folder really is on disk (a folder on the path may not be readable, or its links may loop), ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNRESOLVED_VAR_3}. Check that every folder on that path exists and can be opened, then run this command again.
