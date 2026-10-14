<!--
name: Plugin archive headersHelper disabled by policy
description: >-
  Plugin archive fetch needs a marketplace headersHelper that managed settings
  disable.
ccVersion: 2.1.300
variables:
  - SLASH_COMMAND_PLUGIN_ARCHIVE_HEADERS_HELPER_DISABLED_BY_POLICY_VAR_0
-->
"${SLASH_COMMAND_PLUGIN_ARCHIVE_HEADERS_HELPER_DISABLED_BY_POLICY_VAR_0}" fetches its archive through a marketplace-declared headersHelper command, and your organization's managed settings disable marketplace-declared commands (disableCommandPluginSources / allowManagedHooksOnly). The plugin was not installed or updated and the command was not run; 
