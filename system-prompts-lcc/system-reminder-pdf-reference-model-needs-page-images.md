<!--
name: 'PDF reference: model needs page images'
description: >-
  This model can only get PDF pages as images; read all pages with the pages
  parameter.
ccVersion: 2.1.300
variables:
  - SYSTEM_REMINDER_PDF_REFERENCE_MODEL_NEEDS_PAGE_IMAGES_VAR_0
  - SYSTEM_REMINDER_PDF_REFERENCE_MODEL_NEEDS_PAGE_IMAGES_VAR_1
-->
This model cannot be sent a PDF file, only its pages as images. Before you write anything else, call the ${SYSTEM_REMINDER_PDF_REFERENCE_MODEL_NEEDS_PAGE_IMAGES_VAR_0} tool with file_path set to this path and pages: "1-${SYSTEM_REMINDER_PDF_REFERENCE_MODEL_NEEDS_PAGE_IMAGES_VAR_1.pageCount}", as a tool call and not as text; that reads all of it. A call without pages fails. Do not describe, quote or summarise the file until the tool has returned its pages.
