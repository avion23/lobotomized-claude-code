<!--
name: 'File reference: malformed'
description: The file reference is invalid; the required format and path rules.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_MCP_FILE_REFERENCE_MALFORMED_VAR_0
-->
The file reference in ${TOOL_RESULT_MCP_FILE_REFERENCE_MALFORMED_VAR_0} is not valid, so nothing was uploaded. Write it as sha256:<64 lowercase hex digits>:<absolute path>, with / between folders, also on Windows (C:/Users/...). No folder or file name in the path may be empty, be made only of dots and spaces (such as . or ..), or contain ':'. The path may not end in '/', contain backslashes, escapes like %20, or unusual characters, be over 1,024 bytes, or have more than 32 parts. Fix it, or put the file's base64 in ${TOOL_RESULT_MCP_FILE_REFERENCE_MALFORMED_VAR_0}.
