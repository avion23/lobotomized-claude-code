<!--
name: 'Sandbox install: profile not readable'
description: 'The profile was not made readable, with the reason and how to apply it.'
ccVersion: 2.1.305
variables:
  - DATA_SANDBOX_INSTALL_PROFILE_NOT_READABLE_VAR_0
-->
 Your user profile was not made readable to sandboxed commands (${DATA_SANDBOX_INSTALL_PROFILE_NOT_READABLE_VAR_0.reason.replace(/\.$/,"")}), so they can read nothing in it; run /sandbox install again, as the user who starts sessions, to apply that.
