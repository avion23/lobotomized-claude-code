<!--
name: 'Sandbox: profile grant blocked by running session'
description: The profile read grant was not changed because sandbox sessions are running.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_PROFILE_GRANT_BLOCKED_BY_SESSION_VAR_0
-->
The read grant on your user profile was not changed: sandbox sessions or commands are running${TOOL_RESULT_BASH_SANDBOX_PROFILE_GRANT_BLOCKED_BY_SESSION_VAR_0}, and the grant is written only while none is, so that no session sees it change. What was granted before is as it was. End them and run it again.
