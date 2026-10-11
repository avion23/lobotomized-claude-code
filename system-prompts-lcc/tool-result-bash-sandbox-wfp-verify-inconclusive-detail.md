<!--
name: 'Tool Result: Bash sandbox WFP verify inconclusive detail'
description: >-
  Continuation of the WFP verify-inconclusive reason naming the probe target,
  its outcome and exit status, with the reinstall hint.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_INCONCLUSIVE_DETAIL_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_INCONCLUSIVE_DETAIL_VAR_1
-->
${TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_INCONCLUSIVE_DETAIL_VAR_0.target} was '${TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_INCONCLUSIVE_DETAIL_VAR_0.egress_probe}' (exit ${TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_INCONCLUSIVE_DETAIL_VAR_1.status}). The fence may be absent. Re-run \`srt-win install\`. (${TOOL_RESULT_BASH_SANDBOX_WFP_VERIFY_INCONCLUSIVE_DETAIL_VAR_1.stderr})
