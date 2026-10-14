<!--
name: 'Read PDF: per-message page limit'
description: 'After context filled, each message may read limited PDF pages.'
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_0
  - TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_1
  - TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_2
  - TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_3
-->
The context has filled up once already. Until you give your answer, each of your messages can read at most ${TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_0} PDF ${TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_1(TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_0,"page")}, counting all of its ${TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_2} calls. "${TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_3}" was not read. Ask for it in later messages, at most ${TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_0} ${TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_1(TOOL_RESULT_READ_PDF_PAGES_PER_MESSAGE_LIMIT_VAR_0,"page")} in each. You need not wait for the user between messages.
