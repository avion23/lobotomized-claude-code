<!--
name: 'Plugin validate: repo root taken to be'
description: 'Note: which folder was taken as repository root and what to check.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_TAKEN_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_TAKEN_VAR_1
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_TAKEN_VAR_2
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_TAKEN_VAR_3
-->
The repository root was taken to be ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_TAKEN_VAR_0(SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_TAKEN_VAR_1.dir,SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_TAKEN_VAR_2)}, the nearest parent folder with a .git folder or file. ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_TAKEN_VAR_3.join(" ")} For a plugin submitted from a git repository, the repository root is the top folder of that repository, with only what is committed there, so check that the folder named above is that top folder.
