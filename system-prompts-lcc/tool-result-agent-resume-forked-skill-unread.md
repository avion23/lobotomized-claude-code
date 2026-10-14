<!--
name: 'Tool Result: Agent resume forked skill unread'
description: >-
  Refuses to resume a forked-skill agent until its skill file has been read
  after a reload
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_AGENT_RESUME_FORKED_SKILL_UNREAD_VAR_0
  - TOOL_RESULT_AGENT_RESUME_FORKED_SKILL_UNREAD_VAR_1
-->
Agent ${TOOL_RESULT_AGENT_RESUME_FORKED_SKILL_UNREAD_VAR_0} ran as forked skill ${TOOL_RESULT_AGENT_RESUME_FORKED_SKILL_UNREAD_VAR_1.skillName}, whose file has not been read since a reload kept it; refusing to resume it before it is. Try again shortly.
