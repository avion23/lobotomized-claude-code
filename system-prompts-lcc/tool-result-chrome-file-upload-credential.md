<!--
name: 'Tool Result: Chrome file upload credential path refused'
description: >-
  Refusal to upload a file whose name or folder is a credential location,
  telling Claude to tell the user it was not uploaded
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_CHROME_FILE_UPLOAD_CREDENTIAL_VAR_0
  - TOOL_RESULT_CHROME_FILE_UPLOAD_CREDENTIAL_VAR_1
-->
Cannot upload "${TOOL_RESULT_CHROME_FILE_UPLOAD_CREDENTIAL_VAR_0(TOOL_RESULT_CHROME_FILE_UPLOAD_CREDENTIAL_VAR_1)}": its name or folder is one that credentials are kept under (such as .env, a .pem or .key file, or .ssh), so it is not uploaded on Claude's word alone. Tell the user it was not uploaded.
