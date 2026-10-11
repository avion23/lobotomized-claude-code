<!--
name: 'Tool result: agent toolset grep rg exit failed'
description: Agent toolset grep error when ripgrep exits with a failure code.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_AGENT_TOOLSET_GREP_RG_EXIT_FAILED_VAR_0
  - TOOL_RESULT_AGENT_TOOLSET_GREP_RG_EXIT_FAILED_VAR_1
-->
grep: rg failed: ${TOOL_RESULT_AGENT_TOOLSET_GREP_RG_EXIT_FAILED_VAR_0||`exit ${TOOL_RESULT_AGENT_TOOLSET_GREP_RG_EXIT_FAILED_VAR_1}`}
