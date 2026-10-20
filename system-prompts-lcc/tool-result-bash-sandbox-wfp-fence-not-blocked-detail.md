<!--
name: 'WFP fence: outbound not blocked detail'
description: >-
  States which direct outbound connect was not blocked and asks to re-run the
  install.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_WFP_FENCE_NOT_BLOCKED_DETAIL_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_WFP_FENCE_NOT_BLOCKED_DETAIL_VAR_1
-->
${TOOL_RESULT_BASH_SANDBOX_WFP_FENCE_NOT_BLOCKED_DETAIL_VAR_0.join(" and ")||"a direct outbound connect"} was not blocked [${TOOL_RESULT_BASH_SANDBOX_WFP_FENCE_NOT_BLOCKED_DETAIL_VAR_1}]. Re-run \`
