<!--
name: 'Slash Command: /usage in cloud session'
description: >-
  /usage result in a cloud session: usage isn't shown in chat; open Settings →
  Usage on claude.ai
ccVersion: 2.1.312
variables:
  - SLASH_COMMAND_USAGE_REMOTE_SESSION_SETTINGS_LINK_VAR_0
  - SLASH_COMMAND_USAGE_REMOTE_SESSION_SETTINGS_LINK_VAR_1
  - SLASH_COMMAND_USAGE_REMOTE_SESSION_SETTINGS_LINK_VAR_2
-->
Usage isn't shown in this chat. To see it, open Settings → Usage on claude.ai: ${SLASH_COMMAND_USAGE_REMOTE_SESSION_SETTINGS_LINK_VAR_0(SLASH_COMMAND_USAGE_REMOTE_SESSION_SETTINGS_LINK_VAR_1,SLASH_COMMAND_USAGE_REMOTE_SESSION_SETTINGS_LINK_VAR_2.SESSION_INGRESS_URL)}/settings/usage
