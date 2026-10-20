<!--
name: 'Plugin validate: MCP config too large'
description: 'Finding: MCP config over the size cap, not checked.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_MCP_CONFIG_TOO_LARGE_VAR_0
-->
MCP config is larger than ${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_MCP_CONFIG_TOO_LARGE_VAR_0} bytes and was not read. The loader reads it anyway, so none of its servers were checked.
