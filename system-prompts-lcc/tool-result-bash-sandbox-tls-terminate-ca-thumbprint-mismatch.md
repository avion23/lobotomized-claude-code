<!--
name: 'Tool Result: Bash sandbox tlsTerminate CA thumbprint mismatch'
description: >-
  Sandbox init failure reason when the Windows sandbox user trusts a different
  CA than this session's tlsTerminate CA; surfaces in the Bash tool error
  'Sandbox is required but failed to initialize'.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_SANDBOX_TLS_TERMINATE_CA_THUMBPRINT_MISMATCH_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_TLS_TERMINATE_CA_THUMBPRINT_MISMATCH_VAR_1
  - TOOL_RESULT_BASH_SANDBOX_TLS_TERMINATE_CA_THUMBPRINT_MISMATCH_VAR_2
-->
tlsTerminate on Windows: the sandbox's installed CA (thumb=${TOOL_RESULT_BASH_SANDBOX_TLS_TERMINATE_CA_THUMBPRINT_MISMATCH_VAR_0.thumb}) doesn't match this session's CA (thumb=${TOOL_RESULT_BASH_SANDBOX_TLS_TERMINATE_CA_THUMBPRINT_MISMATCH_VAR_1}). Run \`srt-win user trust-ca ${TOOL_RESULT_BASH_SANDBOX_TLS_TERMINATE_CA_THUMBPRINT_MISMATCH_VAR_2.certPath}\` to update it.
