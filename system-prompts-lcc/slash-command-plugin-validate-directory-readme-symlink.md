<!--
name: 'Plugin validate: README is a symlink'
description: Note that a symlinked README does not count; replace with a file.
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_README_SYMLINK_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_README_SYMLINK_VAR_1
-->
${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_README_SYMLINK_VAR_0(SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_README_SYMLINK_VAR_1,200)} in this folder is a symbolic link. These checks do not follow links and the directory drops them, so it does not count as the plugin's README, and a README at the repository root does not stand in for it. Replace the link with a regular file.
