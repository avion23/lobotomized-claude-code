<!--
name: 'Tool Result: Memory file path has invisible or control characters'
description: >-
  Refuses a memory-file write because its path contains invisible or control
  characters, names them, and tells Claude to rename the file and write it
  again.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_MEMORY_PATH_INVISIBLE_CONTROL_CHARACTERS_VAR_0
  - TOOL_RESULT_MEMORY_PATH_INVISIBLE_CONTROL_CHARACTERS_VAR_1
-->
This memory file's path contains invisible or control characters (${TOOL_RESULT_MEMORY_PATH_INVISIBLE_CONTROL_CHARACTERS_VAR_0(TOOL_RESULT_MEMORY_PATH_INVISIBLE_CONTROL_CHARACTERS_VAR_1)}). Name it without them and write the file again; nothing was written.
