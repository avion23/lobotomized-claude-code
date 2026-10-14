<!--
name: 'Data: Prompt submit slash command line change ignored'
description: >-
  Notice that a hook changed a slash command's typed line and the change is
  never applied
ccVersion: 2.1.299
variables:
  - DATA_PROMPT_SUBMIT_SLASH_COMMAND_LINE_CHANGE_IGNORED_VAR_0
-->
prompt.submit: ${DATA_PROMPT_SUBMIT_SLASH_COMMAND_LINE_CHANGE_IGNORED_VAR_0()} changed a slash command's typed line. That change is never applied: its arguments are changed at command.run, a skill body at skill.prompt.
