<!--
name: allowLocalBinding fixed at initialize
description: >-
  allowLocalBinding differs from the verified loopback mode; on Windows it is
  fixed by install and initialize.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_LOOPBACK_FIXED_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_LOOPBACK_FIXED_VAR_1
  - TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_LOOPBACK_FIXED_VAR_2
-->
network.allowLocalBinding asks for loopback ${TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_LOOPBACK_FIXED_VAR_0(TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_LOOPBACK_FIXED_VAR_1)}, but this session verified the network fence with loopback ${TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_LOOPBACK_FIXED_VAR_0(TOOL_RESULT_BASH_SANDBOX_ALLOW_LOCAL_BINDING_LOOPBACK_FIXED_VAR_2)}. On Windows the loopback mode is fixed by the install and checked at initialize(): it cannot change for one command or through updateConfig(). Call reset() then initialize() with the new value; the installed mode must match it.
