<!--
name: 'srt-win: kept grants in use'
description: srt-win removed nothing because sandbox sessions or commands are running.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_SRT_WIN_KEPT_GRANTS_IN_USE_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_SRT_WIN_KEPT_GRANTS_IN_USE_VAR_1
-->
srt-win ${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_KEPT_GRANTS_IN_USE_VAR_0.slice(0,2).join(" ")} removed nothing: sandbox sessions or commands are running${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_KEPT_GRANTS_IN_USE_VAR_1}, and what they run on is not taken from under them. End them and run it again.
