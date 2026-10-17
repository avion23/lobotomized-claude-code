<!--
name: 'Tool result: Read image file too large'
description: >-
  Read tool error when a file is over the image read limit, suggesting resizing
  or exporting a smaller copy.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_READ_IMAGE_FILE_TOO_LARGE_VAR_0
  - TOOL_RESULT_READ_IMAGE_FILE_TOO_LARGE_VAR_1
  - TOOL_RESULT_READ_IMAGE_FILE_TOO_LARGE_VAR_2
-->
File is too large to read as an image (the limit is ${TOOL_RESULT_READ_IMAGE_FILE_TOO_LARGE_VAR_0(TOOL_RESULT_READ_IMAGE_FILE_TOO_LARGE_VAR_1)}): ${TOOL_RESULT_READ_IMAGE_FILE_TOO_LARGE_VAR_2}. If it is an image, resize it or export a smaller copy, then read that.
