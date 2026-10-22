<!--
name: 'Slash Command: sandbox settings locked'
description: >-
  /sandbox error: settings overridden by higher-priority config, optional extra
  reason.
ccVersion: 2.1.308
variables:
  - SLASH_COMMAND_SANDBOX_SETTINGS_LOCKED_BY_POLICY_VAR_0
-->
Error: Sandbox settings are overridden by a higher-priority configuration and cannot be changed locally.${SLASH_COMMAND_SANDBOX_SETTINGS_LOCKED_BY_POLICY_VAR_0===void 0?"":`
${SLASH_COMMAND_SANDBOX_SETTINGS_LOCKED_BY_POLICY_VAR_0}`}
