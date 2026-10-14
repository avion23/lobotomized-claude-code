<!--
name: 'PDF pages extracted: more pages hint'
description: Suffix stating total pages and suggesting the next pages range.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_PDF_PAGES_EXTRACTED_MORE_PAGES_HINT_VAR_0
  - TOOL_RESULT_PDF_PAGES_EXTRACTED_MORE_PAGES_HINT_VAR_1
-->
. This PDF has ${TOOL_RESULT_PDF_PAGES_EXTRACTED_MORE_PAGES_HINT_VAR_0.totalPages} pages. These are pages 1-${TOOL_RESULT_PDF_PAGES_EXTRACTED_MORE_PAGES_HINT_VAR_0.file.count}. Use the pages parameter to read other pages (e.g., pages: "${TOOL_RESULT_PDF_PAGES_EXTRACTED_MORE_PAGES_HINT_VAR_0.file.count+1}-${TOOL_RESULT_PDF_PAGES_EXTRACTED_MORE_PAGES_HINT_VAR_1.min(2*TOOL_RESULT_PDF_PAGES_EXTRACTED_MORE_PAGES_HINT_VAR_0.file.count,TOOL_RESULT_PDF_PAGES_EXTRACTED_MORE_PAGES_HINT_VAR_0.totalPages)}").
