<!--
name: 'Tool Result: ProposeSkills new name of user skill'
description: >-
  Validation error when a new skill name collides with a user skill, suggesting
  an improvement
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_PROPOSESKILLS_NEW_NAME_OF_USER_SKILL_VAR_0
  - TOOL_RESULT_PROPOSESKILLS_NEW_NAME_OF_USER_SKILL_VAR_1
-->
${TOOL_RESULT_PROPOSESKILLS_NEW_NAME_OF_USER_SKILL_VAR_0.name} is the name of ${TOOL_RESULT_PROPOSESKILLS_NEW_NAME_OF_USER_SKILL_VAR_1.name}, one of the user's own skills, so a new skill saved under it would replace that skill. To change it, read its SKILL.md and propose kind "improvement" with target ${TOOL_RESULT_PROPOSESKILLS_NEW_NAME_OF_USER_SKILL_VAR_1.name}; otherwise propose this under a name of its own.
