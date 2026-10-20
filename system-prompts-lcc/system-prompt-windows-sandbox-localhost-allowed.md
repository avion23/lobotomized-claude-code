<!--
name: 'Windows sandbox: localhost allowed'
description: >-
  With allowLocalBinding on, sandboxed commands can reach localhost on any port
  except one; off-machine traffic goes through the proxy.
ccVersion: 2.1.305
variables:
  - SYSTEM_PROMPT_WINDOWS_SANDBOX_LOCALHOST_ALLOWED_VAR_0
-->
On Windows, sandboxed commands can connect to localhost (127.0.0.1 or ::1) on any port except ${SYSTEM_PROMPT_WINDOWS_SANDBOX_LOCALHOST_ALLOWED_VAR_0}. Nothing off this machine is reachable directly; that goes through the sandbox proxy and \`sandbox.network.allowedDomains\`.
