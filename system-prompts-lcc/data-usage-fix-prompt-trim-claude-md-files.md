<!--
name: 'Usage fix: shorten CLAUDE.md files'
description: Prompt asking to shorten the CLAUDE.md files that load in a project.
ccVersion: 2.1.305
variables:
  - DATA_USAGE_FIX_PROMPT_TRIM_CLAUDE_MD_FILES_VAR_0
  - DATA_USAGE_FIX_PROMPT_TRIM_CLAUDE_MD_FILES_VAR_1
-->
Shorten the CLAUDE.md files that load in \`${DATA_USAGE_FIX_PROMPT_TRIM_CLAUDE_MD_FILES_VAR_0(DATA_USAGE_FIX_PROMPT_TRIM_CLAUDE_MD_FILES_VAR_1)}\`. Keep the rules most tasks need and move the rest into files they point to.
