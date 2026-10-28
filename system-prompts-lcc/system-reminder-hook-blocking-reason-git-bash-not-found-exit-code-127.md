<!--
name: 'Hook blocking reason (Git Bash not found, exit code 127)'
description: >-
  Explains that a hook is blocking because Git Bash was not found and it exited
  with code 127, how the user should fix the hook's command, args and onFailure
  settings, and that Claude must not change the hook
ccVersion: 2.1.310
variables:
  - GIT_FOR_WINDOWS_INSTALL_LINK
-->
blocking because Git Bash wasn't found, so only exit code 0 or 2 counts as this hook's verdict. The hook ended with exit code 127. If its command is only quoted strings, PowerShell started no program. To run a program, install ${GIT_FOR_WINDOWS_INSTALL_LINK} and start a new session, or put the program in "command" and its arguments in "args" ("args": [] if it has none) and set "onFailure" to "block" so that failures still block. To print this text, such as a JSON answer, set "shell" to "powershell". The user needs to do this; Claude should not change the hook.
