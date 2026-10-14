<!--
name: 'Slash Command: Remote Workflow Failed'
description: >-
  Result line when a remote-launched workflow failed, with duration, agent count
  and error.
ccVersion: 2.1.300
variables:
  - SLASH_COMMAND_REMOTE_WORKFLOW_FAILED_VAR_0
-->
workflow failed after ${SLASH_COMMAND_REMOTE_WORKFLOW_FAILED_VAR_0.durationMs}ms (${SLASH_COMMAND_REMOTE_WORKFLOW_FAILED_VAR_0.agentCount} agents): ${SLASH_COMMAND_REMOTE_WORKFLOW_FAILED_VAR_0.error}
