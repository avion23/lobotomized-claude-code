<!--
name: 'WFP verify: plain attempt not blocked'
description: >-
  srt-win wfp verify exited 0 but reported the plain egress attempt as not
  blocked.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_PLAIN_ATTEMPT_NOT_BLOCKED_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_PLAIN_ATTEMPT_NOT_BLOCKED_VAR_1
  - TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_PLAIN_ATTEMPT_NOT_BLOCKED_VAR_2
-->
exited 0 but reported the plain attempt as '${TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_PLAIN_ATTEMPT_NOT_BLOCKED_VAR_0.egress_probe??"missing"}' [${TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_PLAIN_ATTEMPT_NOT_BLOCKED_VAR_1}]. (${TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_PLAIN_ATTEMPT_NOT_BLOCKED_VAR_2.stderr})
