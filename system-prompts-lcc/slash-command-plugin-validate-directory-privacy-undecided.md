<!--
name: 'Plugin validate: privacy warning undecided'
description: 'Note: the privacy warning can''t be ruled out until files are read.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_PRIVACY_UNDECIDED_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_PRIVACY_UNDECIDED_VAR_1
-->
No remote service was seen in what these checks could read, and plugin.json sets no privacy policy URL that they accept, so the directory's privacy warning (PRIVACY_URL_MISSING) cannot be ruled out until the ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_PRIVACY_UNDECIDED_VAR_0.length===1?"file":"files"} named above can be read in full. Fix that first, or ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_PRIVACY_UNDECIDED_VAR_1}.
