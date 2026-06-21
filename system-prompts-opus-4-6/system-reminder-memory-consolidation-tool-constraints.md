<!--
name: 'System Reminder: Memory consolidation tool constraints'
description: >-
  Restricts the memory consolidation job to read-only shell access plus deleting
  memory files and lists sessions to review
ccVersion: 2.1.178
variables:
  - SESSIONS_TO_REVIEW
  - SESSION_ID
-->


Tool constraints for this run: shell is read-only (\`ls\`, \`find\`, \`grep\`, \`cat\`, \`stat\`, \`wc\`, \`head\`, \`tail\`, and similar) plus deleting \`.md\` paths inside the memory directory. Anything else that writes, redirects to a file, or modifies state is denied.

Sessions since last consolidation (${SESSIONS_TO_REVIEW.length}):
${SESSIONS_TO_REVIEW.map((SESSION_ID)=>`- ${SESSION_ID}`).join(`
`)}
