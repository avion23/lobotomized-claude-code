<!--
name: 'Profile grant skip reason: session owner mismatch'
description: >-
  The install ran as a different account than the session owner, so granting
  would open the wrong profile.
ccVersion: 2.1.305
variables:
  - DATA_SANDBOX_PROFILE_GRANT_SKIP_REASON_SESSION_OWNER_MISMATCH_VAR_0
  - DATA_SANDBOX_PROFILE_GRANT_SKIP_REASON_SESSION_OWNER_MISMATCH_VAR_1
-->
the install ran as ${DATA_SANDBOX_PROFILE_GRANT_SKIP_REASON_SESSION_OWNER_MISMATCH_VAR_0.realUserSid} in a session that belongs to ${DATA_SANDBOX_PROFILE_GRANT_SKIP_REASON_SESSION_OWNER_MISMATCH_VAR_0.sessionUserSid}; granting would open the installing account's profile, not the session owner's; ${DATA_SANDBOX_PROFILE_GRANT_SKIP_REASON_SESSION_OWNER_MISMATCH_VAR_1}
