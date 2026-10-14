<!--
name: 'PDF reference: read by pages'
description: Tells the model to read a large PDF by page ranges before answering.
ccVersion: 2.1.300
variables:
  - SYSTEM_REMINDER_PDF_REFERENCE_READ_BY_PAGES_VAR_0
  - SYSTEM_REMINDER_PDF_REFERENCE_READ_BY_PAGES_VAR_1
-->
Before you write anything else, call the ${SYSTEM_REMINDER_PDF_REFERENCE_READ_BY_PAGES_VAR_0} tool with file_path set to this path and a range of a few pages (for example pages: "1-5"), as a tool call and not as text. A call without pages fails. Then read on, about five pages a call (${SYSTEM_REMINDER_PDF_REFERENCE_READ_BY_PAGES_VAR_1} at most), until you have seen what the request needs. Do not describe, quote or summarise any page that the tool has not returned. If you answer from part of the file, tell the user which pages you read.
