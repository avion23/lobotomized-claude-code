<!--
name: 'Tool Result: memory write content secrets blocked'
description: >-
  Refusal returned to the model when a memory-write tool call's content matched
  secret-detection patterns.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_MEMORY_WRITE_CONTENT_SECRETS_BLOCKED_VAR_0
  - TOOL_RESULT_MEMORY_WRITE_CONTENT_SECRETS_BLOCKED_VAR_1
  - TOOL_RESULT_MEMORY_WRITE_CONTENT_SECRETS_BLOCKED_VAR_2
-->
Content contains potential secrets (${TOOL_RESULT_MEMORY_WRITE_CONTENT_SECRETS_BLOCKED_VAR_0(TOOL_RESULT_MEMORY_WRITE_CONTENT_SECRETS_BLOCKED_VAR_1.map((TOOL_RESULT_MEMORY_WRITE_CONTENT_SECRETS_BLOCKED_VAR_2)=>TOOL_RESULT_MEMORY_WRITE_CONTENT_SECRETS_BLOCKED_VAR_2.label)).join(", ")}) and cannot be written to memory. Memory stores are never a place for credentials, and project stores are shared with every collaborator. Remove the sensitive content and try again.
