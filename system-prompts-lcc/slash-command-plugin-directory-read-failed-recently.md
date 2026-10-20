<!--
name: 'Plugin directory: read failed recently'
description: >-
  The Directory could not be read a short while ago and unattended work waits
  before asking again.
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_DIRECTORY_READ_FAILED_RECENTLY_VAR_0
  - SLASH_COMMAND_PLUGIN_DIRECTORY_READ_FAILED_RECENTLY_VAR_1
  - SLASH_COMMAND_PLUGIN_DIRECTORY_READ_FAILED_RECENTLY_VAR_2
-->
it could not be read a short while ago (${SLASH_COMMAND_PLUGIN_DIRECTORY_READ_FAILED_RECENTLY_VAR_0.reason}), and work that runs by itself does not ask it again before ${SLASH_COMMAND_PLUGIN_DIRECTORY_READ_FAILED_RECENTLY_VAR_1(SLASH_COMMAND_PLUGIN_DIRECTORY_READ_FAILED_RECENTLY_VAR_2)}
