<!--
name: 'Skill: Claude API language undetected (security guide exception)'
description: >-
  Says no language is needed for comparing a Managed Agents deployment with the
  security guide; otherwise ask the user which language they use
ccVersion: 2.1.304
variables:
  - SKILL_CLAUDE_API_LANGUAGE_UNDETECTED_SECURITY_GUIDE_EXCEPTION_VAR_0
-->
If the request is to compare a Managed Agents deployment with the published security guide, none is needed: ${SKILL_CLAUDE_API_LANGUAGE_UNDETECTED_SECURITY_GUIDE_EXCEPTION_VAR_0}. Otherwise, ask the user which language they are using (see Language Detection above)
