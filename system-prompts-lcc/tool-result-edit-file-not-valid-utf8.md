<!--
name: 'Tool Result: Edit file unsupported encoding'
description: >-
  Refuses to write a file in an encoding the tools do not write and suggests an
  encoding-preserving shell command or asking the user
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_EDIT_FILE_NOT_VALID_UTF8_VAR_0
  - TOOL_RESULT_EDIT_FILE_NOT_VALID_UTF8_VAR_1
-->
File ${TOOL_RESULT_EDIT_FILE_NOT_VALID_UTF8_VAR_0[TOOL_RESULT_EDIT_FILE_NOT_VALID_UTF8_VAR_1]}. These tools write UTF-8 (or UTF-16LE behind its byte-order mark) and never convert a file's encoding on their own, so nothing was written. If the file is text, make the change with a shell command that reads and writes it in its own encoding (iconv, or PowerShell Get-Content/Set-Content -Encoding), or ask the user whether to convert it to UTF-8 first. To replace the whole file with new UTF-8 text anyway, delete it first, then Write it.
