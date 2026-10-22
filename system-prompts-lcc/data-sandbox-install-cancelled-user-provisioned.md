<!--
name: 'Data: sandbox install cancelled, user provisioned'
description: >-
  Install cancelled at elevation but sandbox user is provisioned; filters
  unverifiable.
ccVersion: 2.1.308
variables:
  - DATA_SANDBOX_INSTALL_CANCELLED_USER_PROVISIONED_VAR_0
-->
Install was cancelled at the elevation prompt, but the sandbox user is already provisioned. Network filters can't be verified from a non-elevated process — run /sandbox to check the current status; if sandboxing doesn't start, run /sandbox install again and approve the elevation prompt.${DATA_SANDBOX_INSTALL_CANCELLED_USER_PROVISIONED_VAR_0===void 0?"":` ${DATA_SANDBOX_INSTALL_CANCELLED_USER_PROVISIONED_VAR_0}`}
