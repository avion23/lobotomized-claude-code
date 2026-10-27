<!--
name: 'Tool Result: Remote tool host VM required but unavailable'
description: Deny when the host runs calls only inside a VM that is unavailable
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_REMOTE_TOOL_HOST_SANDBOX_REQUIRED_UNAVAILABLE_REFUSAL_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_HOST_SANDBOX_REQUIRED_UNAVAILABLE_REFUSAL_VAR_1
-->
${TOOL_RESULT_REMOTE_TOOL_HOST_SANDBOX_REQUIRED_UNAVAILABLE_REFUSAL_VAR_0} is set to run this session's calls only inside a VM, and the VM is not available — nothing ran. Sending the call again will not change that. Tell the user that the VM on ${TOOL_RESULT_REMOTE_TOOL_HOST_SANDBOX_REQUIRED_UNAVAILABLE_REFUSAL_VAR_0} is not available${TOOL_RESULT_REMOTE_TOOL_HOST_SANDBOX_REQUIRED_UNAVAILABLE_REFUSAL_VAR_1===void 0?", and that its owner can check Claude Code there.":`. ${TOOL_RESULT_REMOTE_TOOL_HOST_SANDBOX_REQUIRED_UNAVAILABLE_REFUSAL_VAR_1}`}
