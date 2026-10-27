<!--
name: 'Tool Result: ProposeSkills user skill plugin copy outdated'
description: Validation error when the loaded plugin copy of a user skill is out of date
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_PROPOSESKILLS_USER_SKILL_PLUGIN_COPY_OUTDATED_VAR_0
  - TOOL_RESULT_PROPOSESKILLS_USER_SKILL_PLUGIN_COPY_OUTDATED_VAR_1
-->
${TOOL_RESULT_PROPOSESKILLS_USER_SKILL_PLUGIN_COPY_OUTDATED_VAR_0.target} is ${TOOL_RESULT_PROPOSESKILLS_USER_SKILL_PLUGIN_COPY_OUTDATED_VAR_1.name}, one of the user's own skills, and the copy this session loaded is out of date: its plugin changed or was removed on claude.ai since. Tell the user, and propose the improvement again once the session has reloaded its plugins (usually at their next message), reading its SKILL.md then.
