<!--
name: 'Tool Result: Bash sandbox Windows user not provisioned'
description: >-
  Sandbox init failure reason when the Windows sandbox user or its credential is
  missing; surfaces in the Bash tool error 'Sandbox is required but failed to
  initialize'.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_USER_NOT_PROVISIONED_VAR_0
-->
Windows sandbox user is not provisioned (user=${TOOL_RESULT_BASH_SANDBOX_WINDOWS_USER_NOT_PROVISIONED_VAR_0.provisioned}, cred=${TOOL_RESULT_BASH_SANDBOX_WINDOWS_USER_NOT_PROVISIONED_VAR_0.credPresent}). Run \`npx sandbox-runtime windows-install\` (one UAC prompt) to provision it.
