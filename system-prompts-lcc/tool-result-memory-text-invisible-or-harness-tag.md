<!--
name: 'Tool Result: Memory file text has invisible characters or a harness-tag shape'
description: >-
  Refuses a memory-file write because its text contains invisible/control
  characters and/or text shaped like a harness tag, telling Claude to remove
  them and write the file again.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_MEMORY_TEXT_INVISIBLE_OR_HARNESS_TAG_VAR_0
-->
This memory file's text contains ${TOOL_RESULT_MEMORY_TEXT_INVISIBLE_OR_HARNESS_TAG_VAR_0.join(" and ")}. Remove that and write the file again; nothing was written.
