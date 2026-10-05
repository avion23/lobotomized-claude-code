<!--
name: 'Data: Bash mode command failed message'
description: >-
  User-turn content injected into the conversation when a !-prefixed bash-mode
  command throws, wrapped in bash-stderr.
ccVersion: 2.1.284
variables:
  - DATA_BASH_MODE_COMMAND_FAILED_MESSAGE_VAR_0
  - DATA_BASH_MODE_COMMAND_FAILED_MESSAGE_VAR_1
  - DATA_BASH_MODE_COMMAND_FAILED_MESSAGE_VAR_2
  - DATA_BASH_MODE_COMMAND_FAILED_MESSAGE_VAR_3
-->
<bash-stderr>Command failed: ${DATA_BASH_MODE_COMMAND_FAILED_MESSAGE_VAR_0(DATA_BASH_MODE_COMMAND_FAILED_MESSAGE_VAR_1(DATA_BASH_MODE_COMMAND_FAILED_MESSAGE_VAR_2,DATA_BASH_MODE_COMMAND_FAILED_MESSAGE_VAR_3.session))}</bash-stderr>
