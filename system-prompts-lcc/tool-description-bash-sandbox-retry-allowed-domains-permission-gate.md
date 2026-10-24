<!--
name: 'Tool Description: Bash sandbox retry allowed_domains via permission gate'
description: >-
  Re-run with the host in allowed_domains, else retry with
  dangerouslyDisableSandbox through the permission gate.
ccVersion: 2.1.308
variables:
  - TOOL_DESCRIPTION_BASH_SANDBOX_RETRY_ALLOWED_DOMAINS_PERMISSION_GATE_VAR_0
  - TOOL_DESCRIPTION_BASH_SANDBOX_RETRY_ALLOWED_DOMAINS_PERMISSION_GATE_VAR_1
-->
${TOOL_DESCRIPTION_BASH_SANDBOX_RETRY_ALLOWED_DOMAINS_PERMISSION_GATE_VAR_0}, re-run the command with that host in its \`allowed_domains\` (auto mode)${TOOL_DESCRIPTION_BASH_SANDBOX_RETRY_ALLOWED_DOMAINS_PERMISSION_GATE_VAR_1}; otherwise retry with \`dangerouslyDisableSandbox: true\` directly rather than asking in prose first — the retry itself goes through the permission gate (a user prompt, or the auto-mode classifier when auto mode is active)
