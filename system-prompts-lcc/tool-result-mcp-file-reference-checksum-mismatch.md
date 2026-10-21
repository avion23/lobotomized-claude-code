<!--
name: 'File reference: checksum mismatch'
description: 'The file doesn''t match the SHA-256 in the reference; recompute, never guess.'
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_MCP_FILE_REFERENCE_CHECKSUM_MISMATCH_VAR_0
  - TOOL_RESULT_MCP_FILE_REFERENCE_CHECKSUM_MISMATCH_VAR_1
-->
${TOOL_RESULT_MCP_FILE_REFERENCE_CHECKSUM_MISMATCH_VAR_0} doesn't match the SHA-256 in the reference, so nothing was uploaded. Compute its SHA-256 again (${TOOL_RESULT_MCP_FILE_REFERENCE_CHECKSUM_MISMATCH_VAR_1()}) and make the call again. Never guess the SHA-256.
