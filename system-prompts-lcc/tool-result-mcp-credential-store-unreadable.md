<!--
name: 'Tool Result: MCP credential store unreadable'
description: >-
  Error when stored MCP credentials could not be read so the request did not
  run, with a platform-specific retry hint.
ccVersion: 2.1.308
variables:
  - TOOL_RESULT_MCP_CREDENTIAL_STORE_UNREADABLE_VAR_0
  - TOOL_RESULT_MCP_CREDENTIAL_STORE_UNREADABLE_VAR_1
-->
Couldn't read the stored credentials for MCP server "${TOOL_RESULT_MCP_CREDENTIAL_STORE_UNREADABLE_VAR_0}", so the request didn't run. ${TOOL_RESULT_MCP_CREDENTIAL_STORE_UNREADABLE_VAR_1()==="macos"?"If your Mac's keychain is locked, unlock it, then try again.":"Try again."}
