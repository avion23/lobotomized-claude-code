<!--
name: Hook blocking Git Bash not found
description: >-
  Blocking reason that Git Bash was not found so only exit 0 or 2 counts, with a
  remedy, and that Claude should not change the hook
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_HOOK_BLOCKING_GIT_BASH_NOT_FOUND_VAR_0
  - TOOL_RESULT_HOOK_BLOCKING_GIT_BASH_NOT_FOUND_VAR_1
-->
blocking because Git Bash wasn't found, so only exit code 0 or 2 counts as this hook's verdict. ${TOOL_RESULT_HOOK_BLOCKING_GIT_BASH_NOT_FOUND_VAR_0.type==="command"&&TOOL_RESULT_HOOK_BLOCKING_GIT_BASH_NOT_FOUND_VAR_0.shell==="powershell"?'Make the hook end with exit code 0 or 2, or set "onFailure" to "continue" to let its failures pass.':`${TOOL_RESULT_HOOK_BLOCKING_GIT_BASH_NOT_FOUND_VAR_1} and start a new session, or put the program in "command" and its arguments in "args" ("args": [] if it has none) and set "onFailure" to "block" so that failures still block.`} The user needs to do this; Claude should not change the hook.
