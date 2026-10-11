<!--
name: '/plugin update: plugin directory blocked by organization'
description: >-
  Refresh failure when the built-in plugin directory marketplace is blocked by
  organization policy; its message follows 'Could not check "<plugin>" for
  updates.' and is followed by the administrator's reason.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_PLUGIN_UPDATE_DIRECTORY_BLOCKED_BY_ORGANIZATION_VAR_0
  - SLASH_COMMAND_PLUGIN_UPDATE_DIRECTORY_BLOCKED_BY_ORGANIZATION_VAR_1
-->
${SLASH_COMMAND_PLUGIN_UPDATE_DIRECTORY_BLOCKED_BY_ORGANIZATION_VAR_0} is blocked by your organization. ${SLASH_COMMAND_PLUGIN_UPDATE_DIRECTORY_BLOCKED_BY_ORGANIZATION_VAR_1()}
