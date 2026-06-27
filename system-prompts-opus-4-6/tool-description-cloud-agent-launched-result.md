<!--
name: 'Tool Result: Cloud Agent Launched'
description: >-
  tool_result reporting a launched cloud agent with
  taskId/session_url/output_file and guidance to briefly tell the user and end
  the response.
ccVersion: 2.1.178
variables:
  - TOOL_DESCRIPTION_CLOUD_AGENT_LAUNCHED_RESULT_VAR_0
-->
Cloud agent launched.
taskId: ${TOOL_DESCRIPTION_CLOUD_AGENT_LAUNCHED_RESULT_VAR_0.taskId}
session_url: ${TOOL_DESCRIPTION_CLOUD_AGENT_LAUNCHED_RESULT_VAR_0.sessionUrl}
output_file: ${TOOL_DESCRIPTION_CLOUD_AGENT_LAUNCHED_RESULT_VAR_0.outputFile}
The agent is running in the cloud. You will be notified automatically when it completes.
Briefly tell the user what you launched and end your response.
