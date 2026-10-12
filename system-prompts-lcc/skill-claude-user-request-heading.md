<!--
name: Claude API skill user-request section
description: >-
  User-request section appended to the Claude API skill prompt, quoting unsafe
  request text line by line.
ccVersion: 2.1.296
variables:
  - SKILL_CLAUDE_USER_REQUEST_HEADING_VAR_0
  - SKILL_CLAUDE_USER_REQUEST_HEADING_VAR_1
-->
## User Request

${SKILL_CLAUDE_USER_REQUEST_HEADING_VAR_0?`> ${SKILL_CLAUDE_USER_REQUEST_HEADING_VAR_1.split(/\r\n|[\0-\x08\n-\x1f\x7f-\x9f\u2028\u2029]/).join(`
> `)}`:SKILL_CLAUDE_USER_REQUEST_HEADING_VAR_1}
