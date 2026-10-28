<!--
name: 'Tool Result: Bash same command already backgrounded'
description: Validation refusal when the same command is already running in the background
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_BASH_SAME_COMMAND_ALREADY_BACKGROUNDED_VAR_0
  - TOOL_RESULT_BASH_SAME_COMMAND_ALREADY_BACKGROUNDED_VAR_1
  - TOOL_RESULT_BASH_SAME_COMMAND_ALREADY_BACKGROUNDED_VAR_2
  - TOOL_RESULT_BASH_SAME_COMMAND_ALREADY_BACKGROUNDED_VAR_3
-->
Not started: this same command, in this directory, was moved to the background and has been running for ${TOOL_RESULT_BASH_SAME_COMMAND_ALREADY_BACKGROUNDED_VAR_0(TOOL_RESULT_BASH_SAME_COMMAND_ALREADY_BACKGROUNDED_VAR_1.now()-TOOL_RESULT_BASH_SAME_COMMAND_ALREADY_BACKGROUNDED_VAR_2.startTime,{mostSignificantOnly:!0})} (ID: ${TOOL_RESULT_BASH_SAME_COMMAND_ALREADY_BACKGROUNDED_VAR_2.id}). Its output is being written to: ${TOOL_RESULT_BASH_SAME_COMMAND_ALREADY_BACKGROUNDED_VAR_2.outputFile}. Let it finish, or, to run it again now, stop it first with ${TOOL_RESULT_BASH_SAME_COMMAND_ALREADY_BACKGROUNDED_VAR_3}.
