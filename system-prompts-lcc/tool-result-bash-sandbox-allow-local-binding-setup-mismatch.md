<!--
name: allowLocalBinding differs from set-up
description: >-
  allowLocalBinding asks for local connections differently than the machine
  set-up; set up again.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_SETUP_MISMATCH_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_SETUP_MISMATCH_VAR_1
-->
sandbox.network.allowLocalBinding asks for local connections ${TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_SETUP_MISMATCH_VAR_0[2]==="open"?"on":"off"}, but the sandbox on this machine was set up with them ${TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_SETUP_MISMATCH_VAR_0[1]==="open"?"on":"off"}. Changing that needs set-up again (one elevation prompt). ${TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_SETUP_MISMATCH_VAR_1}
