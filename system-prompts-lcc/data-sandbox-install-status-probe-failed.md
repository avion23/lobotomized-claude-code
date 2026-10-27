<!--
name: 'Data: Sandbox install status probe failed'
description: Error when the installer ran but the sandbox status could not be read back
ccVersion: 2.1.311
variables:
  - DATA_SANDBOX_INSTALL_STATUS_PROBE_FAILED_VAR_0
  - DATA_SANDBOX_INSTALL_STATUS_PROBE_FAILED_VAR_1
-->
The installer ran, but the sandbox status couldn't be read back afterwards: ${DATA_SANDBOX_INSTALL_STATUS_PROBE_FAILED_VAR_0}. ${DATA_SANDBOX_INSTALL_STATUS_PROBE_FAILED_VAR_1.areSandboxSettingsLockedByPolicy()?"Restart Claude Code to check again.":"Run /sandbox to check the current status."}
