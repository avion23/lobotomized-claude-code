<!--
name: 'Windows sandbox: localhost, user alternatives'
description: >-
  Full localhost-blocked guidance (no-retry arm): tell the user how they can
  leave the sandbox.
ccVersion: 2.1.305
variables:
  - SYSTEM_PROMPT_WINDOWS_SANDBOX_LOCALHOST_USER_ALTERNATIVES_VAR_0
  - SYSTEM_PROMPT_WINDOWS_SANDBOX_LOCALHOST_USER_ALTERNATIVES_VAR_1
  - SYSTEM_PROMPT_WINDOWS_SANDBOX_LOCALHOST_USER_ALTERNATIVES_VAR_2
-->
${SYSTEM_PROMPT_WINDOWS_SANDBOX_LOCALHOST_USER_ALTERNATIVES_VAR_0} ${SYSTEM_PROMPT_WINDOWS_SANDBOX_LOCALHOST_USER_ALTERNATIVES_VAR_1} For anything else that needs localhost, tell the user that the sandbox blocks localhost, so the command works only outside the sandbox, without its protection: they can ${SYSTEM_PROMPT_WINDOWS_SANDBOX_LOCALHOST_USER_ALTERNATIVES_VAR_2}; leaving the sandbox is their decision, not yours.
