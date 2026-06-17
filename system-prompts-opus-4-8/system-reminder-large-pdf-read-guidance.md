<!--
name: 'System Reminder: Large PDF read guidance'
description: >-
  Warns that a PDF is too large to read at once and requires reading specific
  page ranges
ccVersion: 2.1.178
variables:
  - PDF_FILE_REFERENCE
  - FORMAT_FILE_SIZE_FN
  - READ_TOOL_NAME
-->
PDF: ${PDF_FILE_REFERENCE.filename} (${PDF_FILE_REFERENCE.pageCount} pages, ${FORMAT_FILE_SIZE_FN(PDF_FILE_REFERENCE.fileSize)}). Too large to read at once — use ${READ_TOOL_NAME} with the pages parameter to read ranges (e.g. pages: "1-5"). Calling ${READ_TOOL_NAME} without pages fails. Start with the first few pages for structure, then read more as needed. Max 20 pages per request.
