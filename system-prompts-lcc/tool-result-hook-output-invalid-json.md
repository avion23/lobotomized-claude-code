<!--
name: 'Tool result: hook output invalid JSON'
description: >-
  Validation error for hook stdout that starts and ends with braces but does not
  parse as JSON; reaches the model inside 'WorktreeCreate hook failed: …' when a
  WorktreeCreate command or MCP-tool hook prints malformed JSON.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_HOOK_OUTPUT_INVALID_JSON_VAR_0
  - TOOL_RESULT_HOOK_OUTPUT_INVALID_JSON_VAR_1
-->
Hook output looks like a JSON object but is not valid JSON — ${TOOL_RESULT_HOOK_OUTPUT_INVALID_JSON_VAR_0(TOOL_RESULT_HOOK_OUTPUT_INVALID_JSON_VAR_1)}. Emit the payload with a JSON encoder (jq, ConvertTo-Json, json.dumps) rather than string concatenation so backslashes and quotes inside strings are escaped.
