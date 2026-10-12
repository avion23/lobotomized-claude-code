<!--
name: 'Claude Code skill: custom agents context'
description: Configured custom agent list in current-build context.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_CLAUDE_CODE_CURRENT_BUILD_CUSTOM_AGENTS_VAR_0
-->
**Custom agents configured:**
${SLASH_COMMAND_CLAUDE_CODE_CURRENT_BUILD_CUSTOM_AGENTS_VAR_0.join(`
`)}
