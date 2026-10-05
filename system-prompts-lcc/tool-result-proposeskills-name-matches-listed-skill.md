<!--
name: 'Tool Result: ProposeSkills name matches a listed skill'
description: >-
  Tells Claude a proposed skill name matches a listed skill whose SKILL.md is
  unread or stale on disk; if it is the user's own skill, saving replaces it
  entirely, so re-read that file (or propose a different name) before calling
  again.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_PROPOSESKILLS_NAME_MATCHES_LISTED_SKILL_VAR_0
  - TOOL_RESULT_PROPOSESKILLS_NAME_MATCHES_LISTED_SKILL_VAR_1
  - TOOL_RESULT_PROPOSESKILLS_NAME_MATCHES_LISTED_SKILL_VAR_2
  - TOOL_RESULT_PROPOSESKILLS_NAME_MATCHES_LISTED_SKILL_VAR_3
-->
The new proposal ${TOOL_RESULT_PROPOSESKILLS_NAME_MATCHES_LISTED_SKILL_VAR_0.written} would be saved under the name of the listed skill ${TOOL_RESULT_PROPOSESKILLS_NAME_MATCHES_LISTED_SKILL_VAR_0.skill.name} (${TOOL_RESULT_PROPOSESKILLS_NAME_MATCHES_LISTED_SKILL_VAR_1}), whose SKILL.md ${TOOL_RESULT_PROPOSESKILLS_NAME_MATCHES_LISTED_SKILL_VAR_2}. If that skill is the user's own, saving this proposal replaces its SKILL.md entirely. Read that whole file ${TOOL_RESULT_PROPOSESKILLS_NAME_MATCHES_LISTED_SKILL_VAR_3==="unread"?"first":"again"}, then call again with a complete SKILL.md that keeps everything worth keeping, or call again under a different name.
