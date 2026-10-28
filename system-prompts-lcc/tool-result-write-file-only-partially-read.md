<!--
name: 'Tool Result: Write refused on partially read file'
description: >-
  Write tool validation error when only the start of the file was read, telling
  Claude to use Edit, or Read it whole (with the full-read parameter) before
  replacing it
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_WRITE_FILE_ONLY_PARTIALLY_READ_VAR_0
  - TOOL_RESULT_WRITE_FILE_ONLY_PARTIALLY_READ_VAR_1
-->
You were given only the start of this file, and nothing shows that you have since read all of it in one call, so a Write could lose the rest. To change part of it, use ${TOOL_RESULT_WRITE_FILE_ONLY_PARTIALLY_READ_VAR_0}. To replace it whole, first Read it in one call with no offset or limit. If Read returns only a page or says the file is too large, Read it again with ${TOOL_RESULT_WRITE_FILE_ONLY_PARTIALLY_READ_VAR_1}: true. If even that cannot return all of it, use ${TOOL_RESULT_WRITE_FILE_ONLY_PARTIALLY_READ_VAR_0}.
