<!--
name: 'Tool Description: Bash sandbox retry allowed_domains'
description: >-
  Re-run with the host in allowed_domains, else retry with
  dangerouslyDisableSandbox without asking.
ccVersion: 2.1.308
variables:
  - TOOL_DESCRIPTION_BASH_SANDBOX_RETRY_ALLOWED_DOMAINS_VAR_0
  - TOOL_DESCRIPTION_BASH_SANDBOX_RETRY_ALLOWED_DOMAINS_VAR_1
-->
${TOOL_DESCRIPTION_BASH_SANDBOX_RETRY_ALLOWED_DOMAINS_VAR_0}, re-run the command with that host in its \`allowed_domains\` (auto mode)${TOOL_DESCRIPTION_BASH_SANDBOX_RETRY_ALLOWED_DOMAINS_VAR_1}; otherwise retry with \`dangerouslyDisableSandbox: true\` (don't ask, just do it)
