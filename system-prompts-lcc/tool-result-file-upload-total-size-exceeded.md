<!--
name: 'Tool Result: file_upload Total Size Exceeded'
description: >-
  Error returned when a Claude-in-Chrome file_upload exceeds the 10 MB
  browser-bridge budget, delivered to the model as a <tool_use_error>
  tool_result telling it to use a smaller file or split the upload.
ccVersion: 2.1.308
variables:
  - TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_0
  - TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_1
  - TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_2
-->
Cannot upload "${TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_0}": total upload size would exceed ${TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_1>=1048576?`${TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_2.floor(TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_1*10/1048576)/10} MB`:TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_1>=1024?`${TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_2.floor(TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_1/1024)} KB`:`${TOOL_RESULT_FILE_UPLOAD_TOTAL_SIZE_EXCEEDED_VAR_1} bytes`}. Use a smaller file, or split across multiple file_upload calls if the page accepts files one at a time.
