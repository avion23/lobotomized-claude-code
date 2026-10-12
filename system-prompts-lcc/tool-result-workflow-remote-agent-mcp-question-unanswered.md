<!--
name: 'Tool Result: workflow remote agent unanswered MCP question'
description: >-
  Workflow agent({isolation:'remote'}) failure when the cloud session has shown
  an unanswered MCP server question for too long.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_WORKFLOW_REMOTE_AGENT_MCP_QUESTION_UNANSWERED_VAR_0
  - TOOL_RESULT_WORKFLOW_REMOTE_AGENT_MCP_QUESTION_UNANSWERED_VAR_1
-->
Cloud session ${TOOL_RESULT_WORKFLOW_REMOTE_AGENT_MCP_QUESTION_UNANSWERED_VAR_0} has shown an unanswered MCP server question for more than ${TOOL_RESULT_WORKFLOW_REMOTE_AGENT_MCP_QUESTION_UNANSWERED_VAR_1/60000} min, and nothing on this machine can answer it, so this run stopped waiting for it. If that server needs to ask the user things, run this agent locally rather than as a cloud session.
