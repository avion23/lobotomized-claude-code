<!--
name: Project write read before replace failed
description: >-
  Error that reading the doc before replacing it failed, to retry once and not
  delete
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_PROJECT_WRITE_READ_BEFORE_REPLACE_FAILED_VAR_0
  - TOOL_RESULT_PROJECT_WRITE_READ_BEFORE_REPLACE_FAILED_VAR_1
-->
Write not done; nothing in the project was changed. Before it replaces a doc, this tool reads the doc's current text, and that read failed: ${TOOL_RESULT_PROJECT_WRITE_READ_BEFORE_REPLACE_FAILED_VAR_0(TOOL_RESULT_PROJECT_WRITE_READ_BEFORE_REPLACE_FAILED_VAR_1).replace(/[.\s]*$/,"")}. Try the same write once more. Do not delete the doc to retry: this tool cannot undo a delete. If it fails again, tell the user that the content was not saved, and offer it to them another way.
