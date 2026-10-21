<!--
name: 'Windows sandbox: localhost, user alternatives'
description: >-
  Full localhost-blocked guidance (no-retry arm): tell the user how they can
  leave the sandbox.
ccVersion: 2.1.305
variables:
  - WINDOWS_LOCALHOST_ACCESS_NOTE
  - WINDOWS_LOCALHOST_WORKAROUNDS_NOTE
  - UNSANDBOXED_COMMAND_ALTERNATIVES
-->
${WINDOWS_LOCALHOST_ACCESS_NOTE} ${WINDOWS_LOCALHOST_WORKAROUNDS_NOTE} For anything else that needs localhost, tell the user that the sandbox blocks localhost, so the command works only outside the sandbox, without its protection: they can ${UNSANDBOXED_COMMAND_ALTERNATIVES}; leaving the sandbox is their decision, not yours.
