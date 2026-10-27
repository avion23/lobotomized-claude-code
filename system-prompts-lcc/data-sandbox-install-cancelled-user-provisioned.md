<!--
name: 'Data: sandbox install cancelled, user provisioned'
description: >-
  Install cancelled at elevation but sandbox user is provisioned; filters
  unverifiable.
ccVersion: 2.1.311
variables:
  - DATA_SANDBOX_INSTALL_CANCELLED_USER_PROVISIONED_VAR_2
  - DATA_SANDBOX_INSTALL_CANCELLED_USER_PROVISIONED_VAR_0
-->
Install was cancelled at the elevation prompt, but the sandbox user is already provisioned. Network filters can't be verified from a non-elevated process${DATA_SANDBOX_INSTALL_CANCELLED_USER_PROVISIONED_VAR_2.areSandboxSettingsLockedByPolicy()?"":" — run /sandbox to check the current status"}; if sandboxing doesn't start, run /sandbox install again and approve the elevation prompt. If you don't have administrator rights, ask your administrator to run the sandbox set-up.${DATA_SANDBOX_INSTALL_CANCELLED_USER_PROVISIONED_VAR_0===void 0?"":` ${DATA_SANDBOX_INSTALL_CANCELLED_USER_PROVISIONED_VAR_0}`}
