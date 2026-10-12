<!--
name: >-
  Skill: mcp served — To read a supporting file this skill references by a
  relativ
description: MCP-backed skill prompt explains reading relative supporting files.
ccVersion: 2.1.296
variables:
  - SKILL_MCP_TO_READ_SUPPORTING_FILE_THIS_SKILL_VAR_0
  - SKILL_MCP_TO_READ_SUPPORTING_FILE_THIS_SKILL_VAR_1
  - SKILL_MCP_TO_READ_SUPPORTING_FILE_THIS_SKILL_VAR_2
-->
To read a supporting file this skill references by a relative path — for example "templates/invoice.md" — call ${SKILL_MCP_TO_READ_SUPPORTING_FILE_THIS_SKILL_VAR_0} with server "${SKILL_MCP_TO_READ_SUPPORTING_FILE_THIS_SKILL_VAR_1.server}" and uri "${SKILL_MCP_TO_READ_SUPPORTING_FILE_THIS_SKILL_VAR_1.uri}/templates/invoice.md".${SKILL_MCP_TO_READ_SUPPORTING_FILE_THIS_SKILL_VAR_2}
