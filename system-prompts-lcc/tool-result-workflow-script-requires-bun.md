<!--
name: 'Tool Result: workflow script requires Bun'
description: >-
  Workflow scripts run only on Bun; this process is not, so the script was not
  started.
ccVersion: 2.1.308
variables:
  - TOOL_RESULT_WORKFLOW_SCRIPT_REQUIRES_BUN_VAR_0
-->
Workflow scripts run only when Claude Code runs on Bun, the JavaScript runtime its native binary is built with. This process is not running on Bun (it reports ${TOOL_RESULT_WORKFLOW_SCRIPT_REQUIRES_BUN_VAR_0.versions.deno!==void 0?`Deno ${TOOL_RESULT_WORKFLOW_SCRIPT_REQUIRES_BUN_VAR_0.versions.deno}`:`Node.js ${TOOL_RESULT_WORKFLOW_SCRIPT_REQUIRES_BUN_VAR_0.version}`}), so the script was not started. To use workflows, run the native \`claude\` binary (the Agent SDK launches it by default) rather than a JavaScript bundle under another runtime.
