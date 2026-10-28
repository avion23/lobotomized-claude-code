<!--
name: 'Slash Command: MCP auth not cleared'
description: >-
  Reports authentication was not cleared because sign-in data remains or the
  store could not be read
ccVersion: 2.1.311
variables:
  - SLASH_COMMAND_MCP_AUTH_NOT_CLEARED_VAR_0
  - SLASH_COMMAND_MCP_AUTH_NOT_CLEARED_VAR_1
-->
Authentication for ${SLASH_COMMAND_MCP_AUTH_NOT_CLEARED_VAR_0(SLASH_COMMAND_MCP_AUTH_NOT_CLEARED_VAR_1.name)} was not cleared: sign-in data is still stored, or the credential store could not be read. Try Clear authentication again.
