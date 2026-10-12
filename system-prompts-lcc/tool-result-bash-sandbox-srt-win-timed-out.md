<!--
name: 'Tool result: sandbox srt-win timed out'
description: Sandbox helper timeout reason
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TIMED_OUT_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TIMED_OUT_VAR_1
-->
srt-win ${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TIMED_OUT_VAR_0.join(" ")} timed out after ${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TIMED_OUT_VAR_1.timeoutMs??15000}ms
