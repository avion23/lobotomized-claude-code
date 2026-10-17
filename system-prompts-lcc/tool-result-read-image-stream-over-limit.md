<!--
name: 'Tool result: Read image stream over limit'
description: >-
  Read tool error when a pipe or device sent more than the image read limit
  without ending.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_READ_IMAGE_STREAM_OVER_LIMIT_VAR_0
  - TOOL_RESULT_READ_IMAGE_STREAM_OVER_LIMIT_VAR_1
  - TOOL_RESULT_READ_IMAGE_STREAM_OVER_LIMIT_VAR_2
-->
Cannot read this as an image: ${TOOL_RESULT_READ_IMAGE_STREAM_OVER_LIMIT_VAR_0} is a pipe or a device, not a regular file, and it sent more than ${TOOL_RESULT_READ_IMAGE_STREAM_OVER_LIMIT_VAR_1(TOOL_RESULT_READ_IMAGE_STREAM_OVER_LIMIT_VAR_2)} without ending.
