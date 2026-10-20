<!--
name: 'Required sandbox lost: command refused'
description: >-
  Required sandbox stopped being available; the command and an unsandboxed retry
  are refused.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_REQUIRED_LOST_REFUSED_VAR_0
-->
Sandbox is required (sandbox.failIfUnavailable) and stopped being available in this session: ${TOOL_RESULT_BASH_SANDBOX_REQUIRED_LOST_REFUSED_VAR_0()}. The command was refused, and so is a request to run it outside the sandbox (dangerouslyDisableSandbox): do not retry it that way. Only commands the user runs themselves with the \`!\` prefix, and commands their settings exclude from the sandbox, still run.
