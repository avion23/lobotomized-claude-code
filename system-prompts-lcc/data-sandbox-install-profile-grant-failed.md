<!--
name: 'Sandbox install: profile grant failed'
description: 'Installed, but the profile could not be made readable; run install again.'
ccVersion: 2.1.305
variables:
  - DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_VAR_0
  - DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_VAR_1
  - DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_VAR_2
  - DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_VAR_3
-->
The sandbox account and network filters are installed, but your user profile could not be made readable to sandboxed commands: ${DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_VAR_0.replace(/\s*No session starts until it is complete[\s\S]*$/,"").replace(/\.$/,"")}. Sandboxed commands will not start until that step completes. Run /sandbox install again to retry.${DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_VAR_1(DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_VAR_2,DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_VAR_3)}
