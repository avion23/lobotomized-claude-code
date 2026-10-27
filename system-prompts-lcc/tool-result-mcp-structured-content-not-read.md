<!--
name: 'Tool Result: MCP structured content not read'
description: >-
  Error when an MCP tool response's structured content was too large or deep to
  read; advises checking whether the tool ran and asking for less data
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_MCP_STRUCTURED_CONTENT_NOT_READ_VAR_0
  - TOOL_RESULT_MCP_STRUCTURED_CONTENT_NOT_READ_VAR_1
-->
The structured content in the response from MCP server "${TOOL_RESULT_MCP_STRUCTURED_CONTENT_NOT_READ_VAR_0}" for tool "${TOOL_RESULT_MCP_STRUCTURED_CONTENT_NOT_READ_VAR_1}" was not read here. This happens most often when it is too large, is nested too deep or holds a number that is too large. The tool may have run: check whether it did before calling it again, and ask for less data.
