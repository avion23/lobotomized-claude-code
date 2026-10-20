<!--
name: allowLocalBinding changed since session start
description: >-
  allowLocalBinding changed but is fixed at set-up on Windows; run /sandbox
  install and restart.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_CHANGED_RESTART_VAR_0
-->
sandbox.network.allowLocalBinding now asks for local connections ${TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_CHANGED_RESTART_VAR_0[1]==="open"?"on":"off"}, but this session started with them ${TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_CHANGED_RESTART_VAR_0[2]==="open"?"on":"off"}, and on Windows that is fixed when the sandbox is set up. Run /sandbox install to change the set-up, then restart Claude Code.
