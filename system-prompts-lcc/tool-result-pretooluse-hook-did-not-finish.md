<!--
name: 'Tool result: PreToolUse hook did not finish'
description: >-
  Blocking error when a PreToolUse hook failed or did not finish, so the call
  was not run, followed by advice.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_PRETOOLUSE_HOOK_DID_NOT_FINISH_VAR_0
  - TOOL_RESULT_PRETOOLUSE_HOOK_DID_NOT_FINISH_VAR_1
  - TOOL_RESULT_PRETOOLUSE_HOOK_DID_NOT_FINISH_VAR_2
-->
[${TOOL_RESULT_PRETOOLUSE_HOOK_DID_NOT_FINISH_VAR_0}]: the hook ${TOOL_RESULT_PRETOOLUSE_HOOK_DID_NOT_FINISH_VAR_1.outcome==="cancelled"?"did not finish":"failed"}, so this call was not run.
${TOOL_RESULT_PRETOOLUSE_HOOK_DID_NOT_FINISH_VAR_2.advice}
