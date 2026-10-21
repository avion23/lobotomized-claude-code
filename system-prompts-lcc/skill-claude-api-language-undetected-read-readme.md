<!--
name: 'Skill: Claude API language undetected (read README)'
description: >-
  No project language detected: resolve the language, then read the matching
  claude-api README or curl examples before anything else
ccVersion: 2.1.304
variables:
  - SKILL_CLAUDE_API_LANGUAGE_UNDETECTED_READ_README_VAR_0
  - SKILL_CLAUDE_API_LANGUAGE_UNDETECTED_READ_README_VAR_1
  - SKILL_CLAUDE_API_LANGUAGE_UNDETECTED_READ_README_VAR_2
-->
No project language was auto-detected. ${SKILL_CLAUDE_API_LANGUAGE_UNDETECTED_READ_README_VAR_0(SKILL_CLAUDE_API_LANGUAGE_UNDETECTED_READ_README_VAR_1,SKILL_CLAUDE_API_LANGUAGE_UNDETECTED_READ_README_VAR_2?"follow the `managed-agents-secure` row in the Managed Agents section above":"see Security Comparison Unavailable above")}, then Read the matching \`{lang}/claude-api/README.md\` (or \`curl/examples.md\` for cURL/raw HTTP or an unsupported language) from the base directory before anything else.
