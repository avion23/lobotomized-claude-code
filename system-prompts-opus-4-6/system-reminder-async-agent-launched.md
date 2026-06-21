<!--
name: 'System Reminder: Async agent launched'
description: >-
  Warns Claude not to duplicate an asynchronously launched agent's work or read
  its full JSONL transcript output file
ccVersion: 2.1.178
variables:
  - AGENT_OUTPUT_FILE
  - READ_TOOL_NAME
-->
Don't duplicate this agent's work — work on non-overlapping files/topics, or briefly tell the user what you launched and end your response.
output_file: ${AGENT_OUTPUT_FILE.outputFile}
Don't ${READ_TOOL_NAME} or tail this file via the shell tool — it's the full subagent JSONL transcript and reading it will overflow your context. If the user asks for progress, say the agent is still running; you'll get a completion notification.
