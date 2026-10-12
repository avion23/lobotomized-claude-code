<!--
name: 'Tool Result: Bash sandbox WFP verify listener bind failed'
description: >-
  Sandbox init failure reason when the WFP egress check could not bind a
  loopback listener outside the permit range; surfaces in the Bash tool error
  'Sandbox is required but failed to initialize'.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_BIND_FAILED_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_BIND_FAILED_VAR_1
-->
verifyWindowsWfpEgress: could not bind a loopback listener outside the WFP permit range [${TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_BIND_FAILED_VAR_0},${TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_BIND_FAILED_VAR_1}] in 5 attempts
