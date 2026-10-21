<!--
name: Profile grant exited nonzero
description: srt-win profile grant exited with a status and its output.
ccVersion: 2.1.305
variables:
  - DATA_SANDBOX_PROFILE_GRANT_EXITED_VAR_0
-->
srt-win profile grant exited ${DATA_SANDBOX_PROFILE_GRANT_EXITED_VAR_0.status}: ${DATA_SANDBOX_PROFILE_GRANT_EXITED_VAR_0.stderr.slice(-2000)||DATA_SANDBOX_PROFILE_GRANT_EXITED_VAR_0.stdout}
