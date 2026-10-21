<!--
name: 'Install: profile grant failed detail'
description: >-
  The sandbox is installed but the profile read grant failed; run the install
  again or forget it.
ccVersion: 2.1.305
variables:
  - DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_DETAIL_VAR_0
  - DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_DETAIL_VAR_1
-->
The Windows sandbox is installed, but the read grant on your user profile ${DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_DETAIL_VAR_0?"did not finish in time":"could not be applied"}: ${DATA_SANDBOX_INSTALL_PROFILE_GRANT_FAILED_DETAIL_VAR_1.message}
No session starts until it is complete. Run the install again, or grantWindowsProfileRead(), to finish it; forgetWindowsProfileRead() removes what was written.
