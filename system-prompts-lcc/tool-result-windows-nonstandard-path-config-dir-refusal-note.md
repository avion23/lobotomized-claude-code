<!--
name: 'Tool Result: Windows non-drive path config-dir refusal note'
description: >-
  Suffix added to a file-write refusal explaining it may only be because a
  Windows path without a drive letter or with strippable names could open a file
  in the config directory
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_WINDOWS_NONSTANDARD_PATH_CONFIG_DIR_REFUSAL_NOTE_VAR_0
-->
${TOOL_RESULT_WINDOWS_NONSTANDARD_PATH_CONFIG_DIR_REFUSAL_NOTE_VAR_0.message.replace(/\.?$/,".")} Claude Code may have refused this only because it reads a Windows path that does not start with a drive letter (a share such as \\\\host\\C$\\x, a device path such as \\\\?\\Volume{GUID}\\x, or \\x), or that holds a name which Windows may strip (such as ".. " or "..."), as each path on this computer that it could open, and one of those is in the config directory. This path, the config directory's path, or a link on the way to either one is written that way. If the file is really somewhere else, such as on another computer, a person can edit it there.
