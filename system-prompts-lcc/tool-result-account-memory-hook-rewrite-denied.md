<!--
name: 'Account memory: hook rewrite denied'
description: >-
  Denial explanation built in eee(e,n,r): `let s=`A ${n} hook rewrote the
  ${e.name} call to the account memory server; a hook may allow or deny such a
  call but not change it. The call is denied.`;return
  t(s,{level:'warn'}),i(...),{behavior:'deny',message:s,decisionReason:{type:'hook',...,reason:s},...}`.
  The SAME string is both logged and embedded verbatim as `message` and
  `decisionReason.reason` of the returned permission decision — matching the
  documented gotcha that decisionReason-derived messages of a returned
  permission decision (ask OR deny) are model-facing, since a denied tool call's
  explanation is what the model reads as its tool_result.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ACCOUNT_MEMORY_HOOK_REWRITE_DENIED_VAR_0
  - TOOL_RESULT_ACCOUNT_MEMORY_HOOK_REWRITE_DENIED_VAR_1
-->
A ${TOOL_RESULT_ACCOUNT_MEMORY_HOOK_REWRITE_DENIED_VAR_0} hook rewrote the ${TOOL_RESULT_ACCOUNT_MEMORY_HOOK_REWRITE_DENIED_VAR_1.name} call to the account memory server; a hook may allow or deny such a call but not change it. The call is denied.
