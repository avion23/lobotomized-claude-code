<!--
name: 'Tool Result: Bash sandbox tlsTerminate CA not installed'
description: >-
  Sandbox init failure reason when tlsTerminate is on but the Windows sandbox
  user has no trusted CA; surfaces in the Bash tool error 'Sandbox is required
  but failed to initialize'.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_SANDBOX_TLS_TERMINATE_CA_NOT_INSTALLED_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_TLS_TERMINATE_CA_NOT_INSTALLED_VAR_1
-->
tlsTerminate on Windows requires the sandbox to be installed with this CA (thumb=${TOOL_RESULT_BASH_SANDBOX_TLS_TERMINATE_CA_NOT_INSTALLED_VAR_0}): run \`srt-win user trust-ca ${TOOL_RESULT_BASH_SANDBOX_TLS_TERMINATE_CA_NOT_INSTALLED_VAR_1.certPath}\`. Per-exec installs into the sandbox user's Root store are not supported.
