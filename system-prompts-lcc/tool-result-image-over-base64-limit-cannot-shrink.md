<!--
name: 'Tool Result: Image over base64 limit, cannot shrink'
description: >-
  Error that an image is over the API's base64 size limit and this session
  cannot shrink images, asking for a smaller file
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_IMAGE_OVER_BASE64_LIMIT_CANNOT_SHRINK_VAR_0
  - TOOL_RESULT_IMAGE_OVER_BASE64_LIMIT_CANNOT_SHRINK_VAR_1
  - TOOL_RESULT_IMAGE_OVER_BASE64_LIMIT_CANNOT_SHRINK_VAR_2
  - TOOL_RESULT_IMAGE_OVER_BASE64_LIMIT_CANNOT_SHRINK_VAR_3
-->
Unable to send image — it is ${TOOL_RESULT_IMAGE_OVER_BASE64_LIMIT_CANNOT_SHRINK_VAR_0(TOOL_RESULT_IMAGE_OVER_BASE64_LIMIT_CANNOT_SHRINK_VAR_1)} in base64, over the API's ${TOOL_RESULT_IMAGE_OVER_BASE64_LIMIT_CANNOT_SHRINK_VAR_0(TOOL_RESULT_IMAGE_OVER_BASE64_LIMIT_CANNOT_SHRINK_VAR_2.maxBase64Size)} limit, and this session cannot shrink images. Make it smaller than ${TOOL_RESULT_IMAGE_OVER_BASE64_LIMIT_CANNOT_SHRINK_VAR_3.floor(TOOL_RESULT_IMAGE_OVER_BASE64_LIMIT_CANNOT_SHRINK_VAR_2.targetRawSize/1024/1024*10)/10}MB and try again.
