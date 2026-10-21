<!--
name: srt-win too old for allowLocalBinding
description: >-
  srt-win does not know --allow-loopback; update it or unset
  network.allowLocalBinding.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TOO_OLD_ALLOW_LOOPBACK_VAR_0
-->
srt-win is too old for network.allowLocalBinding: it does not know \`--allow-loopback\`. Update srt-win (and re-run the install with it), or unset network.allowLocalBinding. (${TOOL_RESULT_BASH_SANDBOX_SRT_WIN_TOO_OLD_ALLOW_LOOPBACK_VAR_0.trim()})
