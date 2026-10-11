<!--
name: 'Tool result: sandbox srt-win trust-ca failed'
description: Sandbox helper trust-ca step failed
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TRUST_CA_FAILED_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TRUST_CA_FAILED_VAR_1
-->
srt-win user trust-ca '${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TRUST_CA_FAILED_VAR_0}' failed (exit ${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TRUST_CA_FAILED_VAR_1.status}): ${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TRUST_CA_FAILED_VAR_1.stderr||TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TRUST_CA_FAILED_VAR_1.stdout}
