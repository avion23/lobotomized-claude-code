<!--
name: 'Tool result: sandbox srt-win nonzero exit'
description: Sandbox helper exited with a nonzero status
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_SANDBOX_SRT_WIN_NONZERO_EXIT_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_SRT_WIN_NONZERO_EXIT_VAR_1
-->
srt-win ${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_NONZERO_EXIT_VAR_0.join(" ")} exited ${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_NONZERO_EXIT_VAR_1.status}: ${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_NONZERO_EXIT_VAR_1.stderr||TOOL_RESULT_BASH_SANDBOX_SRT_WIN_NONZERO_EXIT_VAR_1.stdout}
