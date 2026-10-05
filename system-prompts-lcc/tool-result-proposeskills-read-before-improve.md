<!--
name: 'Propose_skills: read the whole SKILL.md first'
description: >-
  Reworded existing tool_use_error text (added a stale-copy clause) telling the
  model to read SKILL.md files before proposing an update; reusedFrom similarity
  0.95.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_PROPOSESKILLS_READ_BEFORE_IMPROVE_VAR_0
  - TOOL_RESULT_PROPOSESKILLS_READ_BEFORE_IMPROVE_VAR_1
  - TOOL_RESULT_PROPOSESKILLS_READ_BEFORE_IMPROVE_VAR_2
-->
${[...TOOL_RESULT_PROPOSESKILLS_READ_BEFORE_IMPROVE_VAR_0.length>0?[`Existing SKILL.md not read in full yet for ${TOOL_RESULT_PROPOSESKILLS_READ_BEFORE_IMPROVE_VAR_0.join(", ")}.`]:[],...TOOL_RESULT_PROPOSESKILLS_READ_BEFORE_IMPROVE_VAR_1.length>0?[`SKILL.md on disk is newer than the copy read for ${TOOL_RESULT_PROPOSESKILLS_READ_BEFORE_IMPROVE_VAR_1.join(", ")}.`]:[]].join(" ")} A saved proposal replaces a skill's SKILL.md entirely — read ${TOOL_RESULT_PROPOSESKILLS_READ_BEFORE_IMPROVE_VAR_2===1?"that whole file":"those whole files"} ${TOOL_RESULT_PROPOSESKILLS_READ_BEFORE_IMPROVE_VAR_0.length===0?"again":"first"}, then propose the complete updated SKILL.md.
