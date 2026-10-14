<!--
name: 'System Prompt: Windows sandbox allowRead tool folder remedy'
description: >-
  Remedy telling the user to add the tool's folder to
  sandbox.filesystem.allowRead and restart
ccVersion: 2.1.299
variables:
  - SYSTEM_PROMPT_WINDOWS_SANDBOX_ALLOW_READ_TOOL_FOLDER_REMEDY_VAR_0
-->
they can add that tool's own folder to \`sandbox.filesystem.allowRead\` in ${SYSTEM_PROMPT_WINDOWS_SANDBOX_ALLOW_READ_TOOL_FOLDER_REMEDY_VAR_0} (as \`~/...\`, which in a settings file is the user's home, or a full path with backslashes doubled; \`%USERPROFILE%\` is not expanded) and restart Claude Code (an administrator's policy can overrule the entry); sandboxed commands can then read and run everything in it
