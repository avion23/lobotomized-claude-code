<!--
name: WFP filters loopback mode not recorded
description: >-
  WFP filters cannot be used: loopback mode differs from what the install
  recorded.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_WFP_LOOPBACK_MODE_UNRECORDED_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_WFP_LOOPBACK_MODE_UNRECORDED_VAR_1
-->
WFP filters under sublayer ${TOOL_RESULT_BASH_SANDBOX_WFP_LOOPBACK_MODE_UNRECORDED_VAR_0??"(default)"} cannot be used: their loopback mode (${TOOL_RESULT_BASH_SANDBOX_WFP_LOOPBACK_MODE_UNRECORDED_VAR_1.allowLoopback?"open":"closed"}) is not the one the install recorded. Re-run the install for this configuration (one UAC prompt):
  
